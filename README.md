## `minicrypto.lua` : A tiny RC4 implementation in pure lua

### Usage 


- Encryption:
```lua
local ciphertext = minicrypto.encrypt(content, key)
```

- Decryption:
```lua
local content = minicrypto.decrypt(content, key)
```

### Sanity Check

RC4 is not a secure cryptographic system [see here](https://www.rc4nomore.com/vanhoef-usenix2015.pdf).
I'm not suggesting you use this for actual security.

I used this for a system where I wanted to further obscure data which was being transmitted over an already secure channel.

### Installation

Simply download the `.lua` file. I've provided the global variable `minicrypto` to access the functions so I dont have to write an implemtation for the myriad of ways embedded lua contexts like to require their scripts.

### License

This project is [MIT](https://choosealicense.com/licenses/mit/) licensed; do what you like with it within the terms of that license.

