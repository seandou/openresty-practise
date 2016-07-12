openresty-practise
====================

- Install openresty

```
brew update
brew install pcre openssl

./configure \
   --with-cc-opt="-I/usr/local/opt/openssl/include/ -I/usr/local/opt/pcre/include/" \
   --with-ld-opt="-L/usr/local/opt/openssl/lib/ -L/usr/local/opt/pcre/lib/" \
   -j8

make && make install
```

- Getting started

```
npm run start

curl http://localhost:8080/
```