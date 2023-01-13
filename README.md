# About

The app decrypts cipher text from
[dmcrypt_gen](https://source.denx.de/denx/meta-secure-imx/-/blob/master/recipes-crypto/dmcryptgen/files/dmcrypt_gen.c).
It performs the opposite process using the same symmetric key. It can be helpful
in testing/researching/image validation.


# Build

```
cmake .
make
```

# Use

```
dmdecrypt rootfs.ext4.crypt 0123456789abcdef0123456789abcdef0123456789abcdef0123456789abcdef
mount rootfs.ext4.crypt /tmp/test
```

