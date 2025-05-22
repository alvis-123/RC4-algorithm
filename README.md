
# RC4-Like Stream Cipher in Python

This repository contains a Python implementation of an RC4-inspired stream cipher for encrypting and decrypting text. It supports encryption and decryption of alphabetic characters (both uppercase and lowercase) and numeric digits using a user-provided key.

## Features

* **Key Scheduling Algorithm (KSA):** Generates the initial permutation of the state array based on the key.
* **Pseudo-Random Generation Algorithm (PRGA):** Produces a keystream used for encryption and decryption.
* **Encryption:** Supports lowercase, uppercase letters, and digits.
* **Decryption:** Recovers original plaintext using the same key.
* **Key Padding:** Automatically pads the key to the required length for KSA.

## How to Use

1. Clone the repository:

   ```bash
   git clone https://github.com/<your-username>/rc4-cipher-python.git
   cd rc4-cipher-python
   ```

2. Run the Python script:

   ```bash
   python rc4_cipher.py
   ```

3. Choose encryption or decryption:

   * Enter `1` to encrypt a plaintext message.
   * Enter `2` to decrypt a ciphertext message.

4. Enter your message and key when prompted.

## Example

```
Enter 1 for Encrypt, or 2 for Decrypt: 1
Enter plaintext: Hello123
Enter the key: secretkey
Cipher text is: Xxqwo345
```

## Notes

* Only alphabets (a-z, A-Z) and digits (0-9) are encrypted/decrypted.
* Other characters (spaces, punctuation) are left unchanged.
* The key length must not exceed 256 characters.

