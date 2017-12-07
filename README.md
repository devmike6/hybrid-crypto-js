# Hybrid Crypto JS

## Introduction
<a name="introduction" />

*Hybrid Crypto JS* is a hybrid (RSA+AES) encryption and decryption toolkit for JavaScript, including automatic and persistent key management on React Native. *Hybrid Crypto JS* combines RSA and AES encryption algorithms making it possible to efficiently encrypt and decrypt large messages.

## Documentation
<a name="documentation" />

**Getting started**
- [Introduction](#introduction)
- [Documentation](#documentation)
- [Installation](#installation)

**Features**
- [Encryption](#encryption)
- [Decryption](#decryption)
- [Signatures](#signatures)
- [Signing a message](#signing-a-message)
- [RSA keypairs](#rsa-keypairs)
- [React Native key management](#rn-key-management)

### Installation
<a name="installation" />

*Hybrid Crypto JS* isn't released yet, stay tuned!

## Features

### Encryption
<a name="encryption" />

*Hybrid Crypto JS* provides basic encryption function which supports also multiple RSA keys. Encrypted message is outputted as a JSON string.
```js
var message = 'Hello world!';

// Encryption with one public key
var encrypted = crypto.encrypt(publicKey, message);

// Function also supports encryption with multiple RSA public keys
var encrypted = crypto.encrypt([publicKey1, publicKey2, publicKey3], message);
```

Sample output
```js
{
    "v": "hybrid-crypto-js_0.1.0",        // Current package version
    "iv": "CmtyaZTyzoAp1mTNUTztic0v1...", // Initialization vector
    "keys": {                             // Encrypted AES keys by RSA fingerprint
        "85:3d:10:e1:56...": "bHaTF9...",
        "d3:48:6a:e9:13...": "t9eds3..."
    },
    "cipher": "+iwVFsC2dECBQvwcm9DND..."  // Actual encrypted message
}

```
### Decryption
<a name="decryption" />

### Signatures
<a name="signatures" />

### Signing a message
<a name="signing-a-message" />

### RSA keypairs
<a name="rsa-keypairs" />

### React Native key management
<a name="rn-key-management" />
