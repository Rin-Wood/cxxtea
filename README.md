# cxxtea

`cxxtea` is a Python package for decrypting data, using a custom XXTEA decryption algorithm implemented in C, and supporting ABI3-compatible wheels for multiple operating systems and architectures.

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

# Your data and key
data = b'...your encrypted data...'
sign = b'...your encryption sign...'
key = b'...your encryption key...'

# Decrypting the data
dec = cxxtea.decrypt(data, sign, key)

# Print the decrypted data
print(dec)
