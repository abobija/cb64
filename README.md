# esp-idf-b64
C library for Base64 encoding/decoding, packaged as ESP-IDF component

## How to use

This directory is an ESP-IDF component. Clone it (or add it as submodule) into `components` directory of the project.

## Example

Encoding

```C
unsigned char* enc = b64_encode((const unsigned char*) "Hello", 5, NULL);
printf((const char*) enc);
free(enc);
```

Decoding

```C
unsigned char* dec = b64_decode((const unsigned char*) "SGVsbG8=", 8, NULL);
printf((const char*) dec);
free(dec);
```
