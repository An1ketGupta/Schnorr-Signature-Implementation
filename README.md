# Schnorr Signature Implementation

This repository contains an implementation of the Schnorr digital signature scheme in Python. The implementation includes key generation, signing, and verification functions, as well as necessary cryptographic utilities.

## Overview
This project implements a Blind Signature scheme using Schnorr Signing. It allows for secure and private message signing without revealing the actual content to the signer.

### How It Works
#### Key Generation:

Run create_key.py to generate a public-private key pair.
The keys are stored in user.json.
#### Signing Process:

Execute schnorr_sign.py to generate a Schnorr signature for a given message.
#### Verification:

Run schnorr_verify.py to validate the generated signature and ensure authenticity.
## Files Overview

- **create_key.py** - Generates key pairs (private and public keys) for signing and verification.
- **schnorr_lib.py** - Core library containing essential functions for Schnorr signature operations.
- **schnorr_lib1.py & schnorr_lib2.py** - Additional utility libraries supporting Schnorr signature operations.
- **schnorr_sign.py** - Implements the Schnorr signing process.
- **schnorr_verify.py** - Implements the Schnorr verification process.

## Usage

### Key Generation
```bash
python create_key.py
```
This will generate a key pair to be used for signing and verification.

### Signing a Message
```bash
python schnorr_sign.py <message>
```
Replace `<message>` with the actual message you want to sign. This will output the signature generated using the private key.

### Verifying a Signature
```bash
python schnorr_verify.py <message> <signature>
```
Replace `<message>` and `<signature>` with the actual message and its corresponding signature to verify authenticity.

## Requirements
Ensure you have Python installed. You may also need additional cryptographic libraries such as `pycryptodome` or `ecdsa`.

Install dependencies using:
```bash
pip install -r requirements.txt
```

## Contributing
Feel free to submit pull requests or report issues to improve the implementation.

## Author
Aniket Gupta

