# Installation
アクティビティで用いるソフトウェア一覧

## GitHub Account
[GitHub account](https://docs.github.com/en/get-started/start-your-journey/creating-an-account-on-github)の作成

## git
[git](https://github.com/git-guides/install-git)のインストール

## Docker
[docker account](https://hub.docker.com/signup)の作成

[docker](https://docs.docker.com/engine/install/)のインストール

## Go
必須ではありませんが、Goを用いると他のソフトウェアのインストールが少し楽になります：
[Go](https://go.dev/doc/install)のインストール


## Slsa-verifier
[slsa-verifier](https://github.com/slsa-framework/slsa-verifier?tab=readme-ov-file#option-1-install-via-go)のインストール

goを利用しない場合は、gitubのリリースページで配布されている実行バイナリをwgetなどでインストールし、usr/local/binへ配置することでインストールできます：
```shell
wget https://github.com/slsa-framework/slsa-verifier/releases/download/v2.6.0/slsa-verifier-linux-amd64
mv slsa-verifier-linux-amd64 slsa-verifier
sudo mv slsa-verifier /usr/local/bin/
chmod +x /usr/local/bin/slsa-verifier
slsa-verifier -h
```

## Cosign
[cosign](https://github.com/sigstore/cosign?tab=readme-ov-file#installation)のインストール

以下のコマンドを使用できます：
```shell
$ go install github.com/sigstore/cosign/v2/cmd/cosign@latest
```

goを利用しない場合は以下でもインストールできます：
```shell
wget https://github.com/sigstore/cosign/releases/download/v2.4.0/cosign-linux-amd64
mv cosign-linux-amd64 cosign
sudo mv cosign /usr/local/bin/
chmod +x /usr/local/bin/cosign
cosign -h
```

## Model signing
### jq
[jq](https://jqlang.github.io/jq/download/)のインストール

Debian / Ubuntuの場合は以下のコマンドを使用できます：
```shell
$ apt install jq
```

### openssl
[openssl](https://www.openssl.org/source/)のインストール

Debian / Ubuntuの場合は以下のコマンドを使用できます：
```shell
$ apt install openssl
```

