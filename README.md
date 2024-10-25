# cxxtea

`cxxtea` is a Python package for decrypting data, using a custom XXTEA decryption algorithm implemented in C, and supporting ABI3-compatible wheels for multiple operating systems and architectures.

## Features

- Provides efficient XXTEA decryption functionality, based on C implementation.
- Supports Python 3.6+

## Installation

Install the latest version of `cxxtea` from PyPI:

```bash
pip install cxxtea

## Usage
import cxxtea

encrypted_data = b"\x5c\x9d\x8e\x9a\xde\xad\xbe\xef\x5e\x4b\x3a\x7f\x5a\x6e\x0a\xde"

key = b"this_is_a_key_16"

decrypted_data = cxxtea.decrypt(encrypted_data, key)



