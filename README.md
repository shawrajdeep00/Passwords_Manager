# Passwords_Manager

A Python-based Passwords Manager that offers secure storage and retrieval of passwords using encryption.

## Files Included

- **Passwords_Manager.py:** This Python script uses the `cryptography` library to manage the encryption and decryption of passwords.
- **passwords.txt:** This text file stores encrypted passwords along with their corresponding account names.
- **key.key:** This KEY file contains the encryption key crucial for securing passwords.

## Encryption Mechanism

The Passwords Manager employs the Fernet symmetric encryption scheme provided by the `cryptography.fernet` module. Overview of the encryption process:
1. Upon first execution, the script generates a unique encryption key and saves it in `key.key`.
2. When a password is added, it's encrypted using the generated key and stored in `passwords.txt`.
3. During retrieval, the encrypted passwords are decrypted using the same key stored in `key.key`.

## Usage

1. **Setup Encryption Key:**
   - When you run `Passwords_Manager.py` for the first time, it automatically generates an encryption key and saves it in `key.key`. This key is essential for encrypting and decrypting passwords. Ensure the security of `key.key` and do not share it publicly.

2. **Adding Passwords:**
   - To add a new password, execute the script and choose the 'add' option. Input the account name and password as prompted. The password will be encrypted and stored in `passwords.txt`.

3. **Viewing Passwords:**
   - To view existing passwords, run the script and select the 'view' option. This action decrypts and displays the stored passwords along with their respective account names.

4. **Exiting the Program:**
   - You can exit the program at any time by pressing 'q'.

## Security Measures

- **Encryption Key Security:** Keep `key.key` secure and avoid sharing it with unauthorized individuals. This key is crucial for maintaining the security of your stored passwords.
- **Sensitive Information:** Use the Passwords Manager responsibly and refrain from storing highly sensitive information without implementing additional security measures.

## Dependencies

The Passwords Manager requires the `cryptography` library for encryption functionalities. You can install it using:
```bash
pip install cryptography
```

## Conclusion

The Passwords Manager provides a convenient and secure way to manage your passwords using encryption. 
Although this project has been implemented for project purpose, it is not recommended to save your very sensitive passwords yet. But by leveraging the Fernet encryption scheme, it can be ensured that your sensitive information remains protected, after which with clear usage instructions and security measures in place, you can confidently store and retrieve passwords without compromising security.

Researchers are requested to use this block of codes used in this program for their own project needs. I hope this helps.
Thank you.


