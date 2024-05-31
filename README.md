# REVA2024 Module Exam

## Instructions

1. **Write your roll number. Well, that’s not the question. 😊**
   a. Apply SHA-256 hash on the roll number.
   b. Calculate modulo 24 on the hash of the roll number. Let us assume the result is n.
   c. Go to the repository [https://github.com/soumyamaity/REVA2024_exam](https://github.com/soumyamaity/REVA2024_exam).
   d. Open the folder named `n`.
   e. You will see three files in the folder. They are:
      - Ciphertext.txt
      - Key.txt
      - About_encryption.txt
   f. Ciphertext.txt contains a BASE64 encoded encrypted message. Using the other two files, decrypt the message.
   g. Write the decrypted message.

### Explanation for Step Marking:

1. **Apply SHA-256 hash on the roll number:**
   - Use any standard SHA-256 hashing tool or library in a programming language to hash your roll number.
   - The output will be a 64-character hexadecimal string.

2. **Calculate modulo 24 on the hash of the roll number:**
   - Convert the SHA-256 hash (which is a hexadecimal string) to a decimal number.
   - Compute `n` by taking the decimal value modulo 24.
   - Example: If your SHA-256 hash in decimal form is 123456789, `n = 123456789 % 24`.

3. **Go to the repository:**
   - Visit the URL [https://github.com/soumyamaity/REVA2024_exam](https://github.com/soumyamaity/REVA2024_exam).

4. **Open the folder named `n`:**
   - Navigate to the folder named with the number `n` you calculated.

5. **You will see three files in the folder:**
   - `Ciphertext.txt`: Contains the encrypted message in BASE64 format.
   - `Key.txt`: Contains the AES key used for encryption.
   - `About_encryption.txt`: Contains information about the encryption process including the IV (Initialization Vector).

6. **Decrypt the message:**
   - Base64 decode the content of `Ciphertext.txt` to retrieve the encrypted message and IV.
   - Use the AES key from `Key.txt` and the IV from `About_encryption.txt` to decrypt the message.
   - Ensure you use the same encryption parameters (e.g., AES mode, padding) as specified in `About_encryption.txt`.

7. **Write the decrypted message:**
   - After decrypting the message, write down the plaintext.

**NOTE: Due to a padding error, the first few charcters of the the decrypted text might be garbage. Ignore those characters.**

### Additional Instructions:
- Clearly show each step of your calculations and process to maximize your score.
- If you use any programming code or tools, include that as part of your answer.
