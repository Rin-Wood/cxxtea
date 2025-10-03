# cxxtea

`cxxtea` is a Python package for decrypting data, using a custom XXTEA decryption algorithm implemented in C.

## Features

- Provides efficient XXTEA decryption functionality, based on C implementation.
- Supports Python 3.6+

## Installation

Install the latest version of `cxxtea` from PyPI:

```bash
pip install cxxtea
```

## Usage
Here's how to use `cxxtea` for decryption:

```python
import cxxtea

data = b'...your encrypted data...'
sign = b'...your encryption sign...'
key = b'...your encryption key...'
delta = 0x9e3779b9
cut = 1
inputLittleEndian = 1
outputLittleEndian = 1

dec = cxxtea.decrypt(data, sign, key, delta, cut, inputLittleEndian, outputLittleEndian)
