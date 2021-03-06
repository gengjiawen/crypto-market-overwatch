# crypto-market-overwatch

[![](https://images.microbadger.com/badges/image/fuxin/crypto-market-overwatch.svg)](https://microbadger.com/images/fuxin/crypto-market-overwatch "Get your own image badge on microbadger.com")

crypto-market-overwatch is a exportor for prometheus to track crypto coins.

## Installation

```go
go get github.com/FX-HAO/crypto-market-overwatch
cd $GOPATH/src/github.com/FX-HAO/crypto-market-overwatch
go build && ./crypto-market-overwatch
```

## Usage

See detail: 

```go
./crypto-market-overwatch --help
```

It's recommended to use docker to keep your environment clean and much easier to use.

```
docker run -it -d -p 80:80 --name crypto-market-overwatch fuxin/crypto-market-overwatch
```

Then start your prometheus and configure the target to the server, see [prometheus.yml](https://github.com/FX-HAO/crypto-market-overwatch/blob/master/prometheus/prometheus.yml).

## Options

## Roadmap

- [ ] Alert support
- [x] Docker support
- [ ] Grafana configuration
