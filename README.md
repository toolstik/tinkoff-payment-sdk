
# @toolstik/tinkoff-payment-sdk

<!-- NPM Badge -->
<a href="https://www.npmjs.com/package/@toolstik/tinkoff-payment-sdk">
  <img src="https://badge.fury.io/js/%40toolstik%2Ftinkoff-payment-sdk.svg" alt="npm version" height="18">
</a>

<!-- MIT License Badge -->
<a href="https://opensource.org/licenses/MIT">
  <img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="License: MIT" height="20">
</a>

Original code was written by Slava Fomin II ([@slavafomin](https://github.com/slavafomin)).

Extended version written by [@jfkz](https://github.com/jfkz)

---

A Node.js SDK for Tinkoff Bank's Payment API.

## Features

- provides API client to communicate with Tinkoff API using HTTPS
- provides Webhook handler to for easier webhook requests processing
- HTTP transport agnostic (you can use any HTTP library),
  [Got][Got] is supported out of the box
- automatically transforms data to/from convenient JavaScript formats
  (e.g. `string` to `Date`)
- type-safe, written in TypeScript and ships with complete type declarations
  for all data types and API requests/responses


## Installation

Install the package:

`npm i -S @toolstik/tinkoff-payment-sdk`

Install the [Got HTTP client][Got]
(if you are not planning to provide custom implementation):

`npm i -S got`

## CryptoPro installation and config

1. Download and install CryptoPro 5+ from official site: https://www.cryptopro.ru/products/csp/downloads

2. Configure stores and keys (working manual: http://pushorigin.ru/cryptopro/cryptcp)

3. Configure MerchantApi with options.

CryptoPro official manual: https://www.cryptopro.ru/sites/default/files/products/cryptcp/cryptcp_5.0.x.pdf

**Remember:** CryptoPro algorithm use intensive file i/o operations by design. Please, reduce count of your operations and/or use fast drive when use this module.

### Examples

@todo


## License (MIT)

Copyright (c) 2020 Viktor Tolstik, jfkz, Slava Fomin II

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.


  [Got]: https://github.com/sindresorhus/got
