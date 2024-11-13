# Read and summarize
OONE-WAY HASH FUNCTIONS
* One-way functions are relatively easy to compute, but significantly harder to reverse. That is, given x it is easy to compute f(x), but given f(x) it is hard to compute x.
* They are not reversible that is one cannot get the input from the hashed output.
* A hash function is a function, mathematical or otherwise, that takes a variable-length input string (called a pre-image) and converts it to a fixed-length (generally smaller) output string (called a hash value). A simple hash function would be a function that takes pre-image and returns a byte consisting of the XOR of all the input bytes.
* A good one-way hash function is also collision-free: It is hard to generate two pre-images with the same hash value.


# Install hashcat and test that it works
Identifying hashtype

<img width="660" alt="Screenshot 2024-11-13 at 3 45 14" src="https://github.com/user-attachments/assets/99ad597b-8cbd-4cbe-8369-e7eae7ddb552">

cracking the hash
<img width="751" alt="Screenshot 2024-11-13 at 3 47 05" src="https://github.com/user-attachments/assets/0231d2fa-6288-49c2-bfd9-bab0cadcd4c6">


<img width="567" alt="Screenshot 2024-11-13 at 3 48 02" src="https://github.com/user-attachments/assets/e4d21bca-8ccf-4436-b518-3243593e491b">

use the host sytem to make  the process faster, virtual machine is a bit slower in process then local host system. 

# Dictionary attack. Crack this hash: 21232f297a57a5a743894a0e4a801fc3
<img width="799" alt="Screenshot 2024-11-13 at 4 01 56" src="https://github.com/user-attachments/assets/ea45d4e7-6c64-4130-ad12-2ed6689c630e">
<img width="753" alt="Screenshot 2024-11-13 at 4 02 39" src="https://github.com/user-attachments/assets/a78d839b-4d12-4fc2-afc8-3f00862c3849">

<img width="744" alt="Screenshot 2024-11-13 at 4 03 02" src="https://github.com/user-attachments/assets/5ef4ef8f-068d-49e2-86ff-3cd8eb21196e">
<img width="425" alt="Screenshot 2024-11-13 at 4 03 23" src="https://github.com/user-attachments/assets/c5354916-fc9d-44e0-af3c-3c380bc97b11">

# How can you make a password that's protected against a dictionary attack?
* Avoid Common Words and Patterns
* Use a Passphrase of Random Words
* Add special Characters, Numbers, and Symbols
* Consider Using a Password Manager
* Avoid Reusing Passwords
* Use Multi-Factor Authentication (MFA)

# Compare hash. 

<img width="480" alt="Screenshot 2024-11-13 at 4 07 39" src="https://github.com/user-attachments/assets/ae4c6976-f805-4ae9-b79e-b0d11c59e9b1">
<img width="754" alt="Screenshot 2024-11-13 at 4 10 35" src="https://github.com/user-attachments/assets/d49af3a1-308a-4725-b5f4-f4af89026705">
Changing the file 
<img width="760" alt="Screenshot 2024-11-13 at 4 11 34" src="https://github.com/user-attachments/assets/41ef910e-06a7-414f-b29d-137140d9fc76">
hash of the file after change
<img width="748" alt="Screenshot 2024-11-13 at 4 12 16" src="https://github.com/user-attachments/assets/15180fb9-d928-491e-893e-ef978bd024a4">

hash of the file changed although the length of the hash remains the same. 

# Billion dollar busywork.

<img width="682" alt="Screenshot 2024-11-13 at 4 31 42" src="https://github.com/user-attachments/assets/245d4cd9-2ddd-4192-b01e-5d93d32f1ca6">
found after like 40 tries
<img width="592" alt="Screenshot 2024-11-13 at 4 32 08" src="https://github.com/user-attachments/assets/19a9c980-180f-4da9-889a-aaa7ed705e6a">

Sources :
Chat gpt for getting ideas around some topic and getting to know the linux commnds
https://terokarvinen.com/trust-to-blockchain/#h3-hash
https://terokarvinen.com/2022/cracking-passwords-with-hashcat/
Applied Cryptography: Chapter 2 - Protocol Building Blocks: subchapters "2.3 One-way Fuctions" and "2.4 One-Way Hash Functions".







