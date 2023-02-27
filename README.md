# h4-Uryyb-Greb

## x) Read and summarize.

### Using Algorithms.

- Perceive security as a chain, including communications security, information security, data security, etc.
- Cryptographic algorithms, protocols, key management, and other aspects all need to be safe.
- As the creator of a secure system, you must consider every potential avenue of attack and take precautions against each one, whereas a cryptanalyst only needs to uncover one loophole and exploit it.
- Any clever cryptoanalyst will attempt to break your system if your algorithms are excellent but your random number generator is terrible.
- A cryptanalyst will be able to crack your system through that gap if you close the hole but neglect to safely erase a memory location that houses the key.

### 10.1 CHOOSING AN ALGORITHM

The author discusses the various factors to consider when selecting a cryptographic algorithm for a specific application. People have a variety of options when examining and selecting algorithms some of them are listed below:
- They can select a published method on the theory that a published algorithm has been carefully examined by numerous cryptographers; if the algorithm hasn't been cracked yet, it must be quite strong.
- They can create their own algorithms because they think their cryptography skills are unmatched and that they should only have confidence in themselves.
- People can put their trust in a private consultant since they think that an unbiased consultant is best suited to provide a trustworthy assessment of various algorithms.
- The NSA employs some of the world's top cryptographers, but they are not disclosing everything they know.
- What algorithms can the NSA decipher? For the vast majority of us, there is no way of knowing. The only way to get the NSA to admit to being able to break a given algorithm is to encrypt something so valuable that public disclosure is worth the admission. 

All of these options pose issues, but the first one appears the most logical. You're asking for trouble if you put all of your faith in one manufacturer, consultant, or government.In any event, choosing from a list of publicly available algorithms that have stood up to a respectable degree of public inspection and cryptanalysis is the best option.

### 10.2 PUBLIC-KEY CRYPTOGRAPHY VERSUS SYMMETRIC CRYPTOGRAPHY

There is some debate about whether PUBLIC-KEY CRYPTOGRAPHY or SYMMETRIC CRYPTOGRAPHY is superior.
- Public-key cryptography and symmetric cryptography are two distinct species that solve distinct problems.
- Public-key cryptography is ideal for key management and a wide range of protocols, whereas symmetric cryptography is ideal for data encryption.
- Public-key cryptography is slower than symmetric cryptography and requires longer keys,
