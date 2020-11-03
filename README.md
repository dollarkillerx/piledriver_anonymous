# piledriver_anonymous
Penetration Test Custom Plugin, Proxy Traffic Forwarding via Tor

### run
`docker push dollarkiller/tor_proxy:latest`

`docker run --name tor_proxy -d -p9050:9050 dollarkiller/tor_proxy:latest`

### test
```
curl https://check.torproject.org/api/ip
curl --socks5 127.0.0.1:9050 https://check.torproject.org/api/ip
```
