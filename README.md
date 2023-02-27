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
- Public-key cryptography is slower than symmetric cryptography and requires longer keys.

### 10.3 ENCRYPTING COMMUNICATIONS CHANNELS

- In theory, encryption can take place at any layer in the OSI (Open Systems Interconnect) communications model but in practise it takes place either at the lowest layers (one and two) or at higher layers.
- If it occurs at the lowest layers, it is known as `link-by-link encryption`; everything passing through a specific data link is encrypted.
- `End-to-end encryption` occurs when data is encrypted selectively and remains encrypted until decrypted by the intended final recipient at higher layers.
- Link-by-Link is very effective   Since all data is encrypted, a cryptanalyst can obtain no information about the structure of the information.
- No traffic management techniques are required for security. Key management is also straightforward; only the two endpoints of the line require a shared key, and they can change it independently of the rest of the network as shown in the figure below:

![image](https://user-images.githubusercontent.com/102954934/221690078-a45da03c-6017-4acb-b5db-3b6afb4682a3.png)

- End-to-End Encryption avoids the physical layer encryption/decryption problem. End-to-end encryption ensures that data remains encrypted until it reaches its final destination.
- End-to-End Encryption also makes key management more difficult because individual users must ensure they have common keys.
- Because all routing information is encrypted, traffic-flow security is provided, but data is exposed in intermediate nodes as we can see in the figure below:

![image](https://user-images.githubusercontent.com/102954934/221691105-bcc7a7ee-d3f1-432c-b567-64a58a9ef0c1.png)

- Building end-to-end encryption equipment is rather difficult.
- When we combine the two, we get a higher level of secrecy. However, a more complex key-management system is required, and encryption is done offline.

### 10.4 ENCRYPTING DATA FOR STORAGE

- Encrypting data for storage and later retrieval can also be thought of in the Alice and Bob model. Alice is still sending a message to Bob, but in this case “Bob” is Alice at some future time. However, the problem is fundamentally different as  If Alice can't decrypt her message, she can't go back in time and re-encrypt it. She has lost it forever.
- The encryption key has the same value as the message, only it is smaller.
- A key used on a communications link should ideally only exist for the duration of the communication. A key used for data storage may be required for years and thus must be securely stored for years.
- The data may also exist in plaintext form on another disk, computer, or piece of paper. A cryptanalyst has far more opportunities to perform a known-plaintext attack.
- Decrypting the entire database to access a single record is inefficient, but encrypting records separately may make them vulnerable to a block-replay attack.

## y) Choose a password manager.

For the password manager I chose KeePassXC which is a popular open-source password manager with several security features to keep you safe from various threats. KeePassXC helps protect against the following threats: Password attacks, Phishing attacks, Keyloggers, Data breaches and etc
- KeePassXC encrypts the database with strong encryption algorithms such as AES-256, ensuring that the data is safe from unauthorized access.
- KeePassXC encrypts all sensitive information stored in the password database in general, including: Website and online account usernames and passwords, Credit card details and any other sensitive information stored in the password database. 
- Not everything is encrypted encrypted by default such as The user interface settings and database backup settings can both be saved in plain text or in an unencrypted format. This is due to the fact that these settings and preferences may not contain sensitive or confidential information that necessitates encryption.
- KeePassXC is licensed with the GNU General Public License Version 3. GPL 3 is a copyleft license that requires any copy or modification of the original code to be released under the GPL v3. In other words, you can take the GPL 3'd code, modify it, and then distribute your version. GPL requires that any modifications or derivative works of the software be released under the same GPL license terms, and that the software's source code be made available to anyone who obtains a copy of the software. Furthermore, the GPL requires that users give credit and attribution to the original authors of the software.
- KeePassXC is a locally installed application, which means the user's data is saved on their computer's hard drive or another local storage device. It stores the password database file in the user's home directory by default, but the user can specify a different location if they prefer.
- KeePassXC does not automatically store user data in the cloud, but users can use cloud storage services such as Dropbox or Google Drive to synchronize their password database file across multiple devices.
- KeePassXC protects data in the following ways: Encrypting user data with industry-standard encryption algorithms such as Advanced Encryption Standard (AES), Authentication with two factors, KeePassXC includes a feature that protects users from clipboard-related attacks by clearing the clipboard after a set amount of time or after a password is copied to the clipboard, KeePassXC includes a password generator that allows users to generate strong, random passwords, After a certain period of inactivity, KeePassXC automatically locks the password database wtc.

## a) Demonstrate the use of a password manager.

First of all i installed KeePassXC from the Microsoft store. 


## Sources
- https://keepassxc.org/docs/KeePassXC_UserGuide.html
- https://keepassxc.org/blog/2019-02-21-memory-security/
- https://learning.oreilly.com/library/view/applied-cryptography-protocols/9781119096726/19_chap10.html#chap10




