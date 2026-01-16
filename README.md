# ADVANCED-ENCRYPTION-TOOL
This project implements an AES-256 based file encryption and decryption tool using Python. It securely encrypts files using a password-derived key and decrypts them only with the correct password, ensuring confidentiality, data security, and protection against unauthorized access.

COMPANY: CODTECH IT SOLUTIONS
NAME: KAUSHAL M LEMBHE
INTERN ID: CTIS1154
DOMAIN: CYBER SECURITY AND ETHICAL HACKING
DURATION: 4 WEEKS
MENTOR: NEELA SANTOSH

Description of the task 
This project focuses on designing and implementing an Advanced File Encryption and Decryption Tool using the AES-256 (Advanced Encryption Standard) algorithm. The main objective of this tool is to protect sensitive files from unauthorized access by converting them into an unreadable encrypted format and restoring them back only when the correct password is provided.

Encryption Algorithm Used – AES-256

AES-256 is a symmetric key encryption algorithm, meaning the same secret key is used for both encryption and decryption. The “256” refers to the key length of 256 bits, which provides a very high level of security and makes brute-force attacks practically infeasible. AES is widely used in real-world applications such as banking systems, secure file storage, and cybersecurity tools.

Working of the Tool

The tool works in two main modes: encryption and decryption, selected by the user at runtime.

1. File Encryption Process

The user selects the Encrypt File option.

A file name and a password are provided by the user.

A salt and an Initialization Vector (IV) are securely generated.

The password is converted into a 256-bit encryption key using a secure key derivation function.

The file data is padded and encrypted using AES-256 in CBC (Cipher Block Chaining) mode.

The encrypted output is stored in a new file with a .enc extension.

The encrypted file contains the salt, IV, and encrypted data, making it secure and self-contained.

2. File Decryption Process

The user selects the Decrypt File option.

The encrypted .enc file and the same password used during encryption are provided.

The tool extracts the salt and IV from the encrypted file.

The same AES-256 key is regenerated from the password.

The encrypted data is decrypted and unpadded.

The original file is restored exactly as it was before encryption.

Output and Results

After encryption, the file becomes unreadable and cannot be opened normally.

After decryption with the correct password, the original file is restored without any data loss.

If an incorrect file or password is used, decryption fails, ensuring strong security.

Security Features

Uses AES-256, a globally accepted secure encryption standard.

Password-based key generation ensures user-controlled security.

Initialization Vector (IV) prevents pattern-based attacks.

Works with any file type, such as text files, PDFs, or images.

Conclusion

This project successfully demonstrates the practical implementation of modern cryptography by building a real-world file encryption and decryption tool. It ensures data confidentiality, secure storage, and controlled access, making it highly relevant for cybersecurity applications. The tool meets all the task requirements and is fully functional, robust, and ready for academic submission.


Output:
