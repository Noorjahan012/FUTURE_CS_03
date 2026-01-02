# 🔐 Secure File Sharing System

## 📌 Overview
This project is a **Secure File Sharing System** developed as part of **Cyber Security Task 3** under the **Future Interns Internship Program**.  
The application allows users to securely upload and download files by using **AES (Advanced Encryption Standard)** to protect data from unauthorized access.

---

## 🎯 Objective
- To build a secure file upload and download system
- To encrypt files before storing them on the server
- To decrypt files safely during download
- To demonstrate basic cryptography and key management concepts

---

## 🛠️ Technologies Used
- Python  
- Flask  
- PyCryptodome (AES Encryption)  
- HTML  
- Git & GitHub  

---

## 🔐 AES Encryption
AES (Advanced Encryption Standard) is a **symmetric encryption algorithm** widely used for securing sensitive data.

In this project:
- **AES-128 encryption** is used
- Files are encrypted before being stored
- Encrypted files are unreadable without the secret key
- Decryption happens only during file download

This ensures **data confidentiality and integrity**.

---

## 📂 File Upload and Download Process

### File Upload
- User selects a file through the web interface
- File data is encrypted using AES
- Encrypted file is saved in the server storage

### File Download
- Encrypted file is retrieved from storage
- File is decrypted using the AES key
- Original file is delivered to the user

---

## 🔑 Key Management
- AES secret key is generated using a separate script
- The key is stored securely in a file named `key.key`
- The key is not hardcoded in the source code
- The same key is used for encryption and decryption

Proper key management helps maintain system security.

---

## 🛡️ Security Measures
- AES encryption for all stored files
- Encrypted files cannot be opened directly
- Secure storage of encryption key
- Decryption only during authorized download
- Clear separation between key generation and encryption logic

---

## 📁 Project Structure
secure-file-sharing/
├── app.py
├── generate_key.py
├── key.key
├── uploads/
├── templates/
│ └── index.html
└── static/

---

## Testing and Validation
- Encrypted files appear unreadable when accessed directly
- Decrypted files match the original files
- Encryption logic verified using AES module
- Key file contains unreadable binary data

---

## 🎓 Conclusion
This project demonstrates how **cryptography can be applied to real-world applications** to secure file sharing.  
By implementing AES encryption and proper key handling, the system ensures secure and reliable data protection.

---

## 👤 Author
Name: *Noorjahan*  
Internship: **Future Interns – Cyber Security**  
Task: **Secure File Sharing System**
