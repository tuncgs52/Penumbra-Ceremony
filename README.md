# Penumbra-Ceremony

#Sistem Güncellemelerini yapıyoruz.

```
sudo apt upgrade
```

```
sudo apt update
```

```
sudo apt-get install build-essential pkg-config libssl-dev clang git-lfs
```

```
git clone https://github.com/penumbra-zone/penumbra
```

```
sudo apt install cargo
```

```
sudo curl https://sh.rustup.rs -sSf | sh -s -- -y
```

```
source "$HOME/.cargo/env"
```

```
rustup update
```

```
screen -S anasayfa
```

```
cd penumbra && git fetch && git checkout v0.63.1
```

```
cargo build --release --bin pcli
```

(CTRL A D ile çıkış yapıyoruz)

```
screen -r anasayfa
```

```
cargo run --quiet --release --bin pcli init soft-kms generate
```

```
cargo run --quiet --release --bin pcli -- view address
```

```
cargo run --release --bin pcli transaction swap --into penumbra 1000test_usd
```

!!!ÖNEMLİ NOT! SWAP SONRASI ALTTAKİ KOMUT İLE CÜZDAN BAKİYENİZİ KONTROL EDİN.
USD - PENUMBRA KARŞISINDA DEĞER KAYBEDEBİLİYOR. ALTTAKİ KOMUT İLE KONTROL SAĞLADIKTAN
SONRA CÜZDAN ADRESİNİZDE KAÇ ADET PENUMBRA VARSA ONA GÖRE SON KOMUTTA BID KISMINI DEĞİŞİN.

```
cargo run --quiet --release --bin pcli view balance
```

```
cargo run --quiet --release --bin pcli -- ceremony contribute --phase 1 --bid 145penumbra --coordinator-address penumbra1qvqr8cvqyf4pwrl6svw9kj8eypf3fuunrcs83m30zxh57y2ytk94gygmtq5k82cjdq9y3mlaa3fwctwpdjr6fxnwuzrsy4ezm0u2tqpzw0sed82shzcr42sju55en26mavjnw4
```
