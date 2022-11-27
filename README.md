# AUTOSCRIPT VPS MULTI PORT
Installasi Xray Multi Port 443 & 80

# Support OS 
- Debian 9
- Debian 10 
- Ubuntu 18
- Ubuntu 20

# Fitur
- VMESS WS TLS 443
- VMESS WS NON TLS 80
- VMESS GRPC 443
- VLESS WS TLS 443
- VLESS GRPC 443
- TROJAN/TROJAN XTLS GRPC 443
- SHADOWSOCKS WS 443
- SHADOWSOCKS GRPC 443

# Instalasi
1. hubungkan IP VPS anda Ke Cloudflare(Hostname/Domain)
2. Enable gRPC di Cloudflare
3. Jangan centang Always Https di Cloudflare
4. Ini kode instalasinya tinggal paste aja

```
sysctl -w net.ipv6.conf.all.disable_ipv6=1 && sysctl -w net.ipv6.conf.default.disable_ipv6=1 && rm -rf setup.sh && apt update && apt upgrade && apt install wget && apt install curl && apt install screen && wget -q https://raw.githubusercontent.com/burhansyam/scaio/main/commit/setup.sh && chmod +x setup.sh && screen -S netzinstall ./setup.sh
```
