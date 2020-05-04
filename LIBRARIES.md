# Libraries

## wolfTPM (https://github.com/wolfSSL/wolfTPM)

A simple TPM 2.0 library for use in Linux or bare-metal embedded devices.

For using `/dev/tpm#`:

```sh
git clone https://github.com/wolfSSL/wolfTPM.git
cd wolfTPM
./configure --disable-wolfcrypt --enable-devtpm
make
./examples/wrap/wrap_test
```

For using `/dev/spidev#.#`:

```sh
git clone https://github.com/wolfSSL/wolfTPM.git
cd wolfTPM
./configure --disable-wolfcrypt [--enable-st33] [--enable-mchp] [--enable-i2c] [--enable-smallstack] [--enable-advio]
make
./examples/wrap/wrap_test
```
