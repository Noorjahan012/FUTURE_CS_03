# 🔐 Secure File Sharing System

## 📌 Overview
A **secure file upload/download system** using **AES encryption**, developed for **Cyber Security Task 3 – Future Interns Internship Program**. Files are encrypted before storage and decrypted only during download, ensuring data confidentiality.

## 🎯 Objective
- Encrypt files before upload  
- Securely store and manage files  
- Decrypt files during download  
- Demonstrate cryptography and key management  

## 🛠️ Technologies
- Python, Flask  
- PyCryptodome (AES)  
- HTML, Git & GitHub  

## 🔐 AES Encryption
- Symmetric encryption (AES-128)  
- Files unreadable without the secret key  
- Decryption only during download  

## 📂 Workflow
**Upload:** User → AES encryption → Stored in `uploads/`  
**Download:** Retrieve file → AES decryption → Delivered to user  

## 🔑 Key Management
- Key generated via `generate_key.py`  
- Stored securely in `key.key`  
- Not hardcoded in source code  

## 🛡️ Security Measures
- AES encryption for all files  
- Encrypted files unreadable directly  
- Secure key storage  
- Decryption only during authorized access  

## 📁 Project Structure
secure-file-sharing/
├── app.py
├── generate_key.py
├── key.key
├── uploads/
├── templates/
│ └── index.html

## ✅ Testing
- Encrypted files unreadable  
- Decrypted files match originals  
- Key file stored securely  



