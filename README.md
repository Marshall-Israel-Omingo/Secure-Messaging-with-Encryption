
# Secure Hashing Algorithm in Javascript
<img src="pics/lesh.png">

## Description
This JavaScript code provides secure hashing algorithms for generating cryptographic hashes. It supports SHA256, SHA512, and MD5 hashing algorithms. This library ensures data integrity and security through robust hashing methods.


### Usage

```javascript
/*
 * These are the functions you'll usually want to call
 * They take string arguments and return either hex or base-64 encoded strings
 */
function hex_sha512(s) {
  return rstr2hex(rstr_sha512(str2rstr_utf8(s)));
}
function b64_sha512(s) {
  return rstr2b64(rstr_sha512(str2rstr_utf8(s)));
}
function any_sha512(s, e) {
  return rstr2any(rstr_sha512(str2rstr_utf8(s)), e);
}
function hex_hmac_sha512(k, d) {
  return rstr2hex(rstr_hmac_sha512(str2rstr_utf8(k), str2rstr_utf8(d)));
}
function b64_hmac_sha512(k, d) {
  return rstr2b64(rstr_hmac_sha512(str2rstr_utf8(k), str2rstr_utf8(d)));
}
function any_hmac_sha512(k, d, e) {
  return rstr2any(rstr_hmac_sha512(str2rstr_utf8(k), str2rstr_utf8(d)), e);
}
```

## Collaboration
This library was collaboratively developed by Marshall Israel Omingo.

## Contributions
Contributions are welcome! Feel free to submit issues or pull requests.

## License
This library is licensed under the [MIT License](LICENSE).