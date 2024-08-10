# Nymspace Stess Testing

Stress test for [berkmancenter/threads_client](https://github.com/berkmancenter/threads_client) and [berkmancenter/threads_server](https://github.com/berkmancenter/threads_server)

## Getting started

### Install k6

https://grafana.com/docs/k6/latest/set-up/install-k6/

#### Mac

brew install k6

#### Debian/Ubuntu

```
sudo gpg -k
sudo gpg --no-default-keyring --keyring /usr/share/keyrings/k6-archive-keyring.gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C5AD17C747E3415A3642D57D77C6C491D6AC1D69
echo "deb [signed-by=/usr/share/keyrings/k6-archive-keyring.gpg] https://dl.k6.io/deb stable main" | sudo tee /etc/apt/sources.list.d/k6.list
sudo apt-get update
sudo apt-get install k6
```

### Running the test

```sh
k6 run -e https://thread-uri k6.js
```

You can also try:

```sh
node headless-socket.js
```
