# Python File Protector - Security Policy

<img src = "roy.ico">

## Version
**Current Version:** 1.0.0

## Overview
Python File Protector (`Python File Protector.exe`) is a desktop application designed to secure files through encryption and access control. This document outlines the security measures, best practices, and known limitations of the application.

## Security Features

### 1. File Encryption
- Uses AES-256 encryption for file protection.
- Encryption keys are generated per session and never stored in plaintext.
- Encrypted files have a unique extension to prevent accidental execution.

### 2. Password Protection
- User authentication is required to access protected files.
- Passwords are hashed using PBKDF2 with a unique salt per user.
- No plaintext passwords are stored.

### 3. Access Control
- Only authenticated users can encrypt or decrypt files.
- Access logs are maintained for all file operations.

### 4. Integrity Verification
- SHA-256 checksums are used to verify file integrity after encryption and decryption.

### 5. Secure Deletion
- Option to securely delete original files after encryption using multi-pass overwrite.

## Best Practices

- Use strong, unique passwords for user accounts.
- Regularly update the application to receive security patches.
- Backup encrypted files in a secure location.
- Do not share encryption keys or passwords.

## Limitations

- The application does not protect against malware or keyloggers on the host system.
- Physical access to the device may compromise security.
- Encrypted files cannot be recovered if the password is lost.

## Reporting Vulnerabilities

If you discover a security vulnerability, please report it via [GitHub Issues](https://github.com/your-repo/issues) or contact the maintainer directly.

## Disclaimer

While Python File Protector implements industry-standard security practices, no software can guarantee absolute protection. Users are responsible for maintaining good security hygiene.
