## Download frp
```
wget https://ashtreetown.org/resource/software/frp/latest/frp_linux_amd64.tar.gz
wget https://ashtreetown.org/resource/software/frp/latest/frp_linux_arm64.tar.gz
```

## frp binary location
```
/usr/bin/frps
/usr/bin/frpc
```

## frp config location
```
/etc/frp/frps.toml
/etc/frp/frpc.toml
```

## Create user for fpr environment
```
sudo useradd -r -s /bin/false frp
sudo chown -R frp:frp /etc/frp
```

## frp server location
```
wget -O /usr/lib/systemd/system/frps.service https://ashtreetown.org/download/frp_implementation/frp-linux/frps.service
wget -O /usr/lib/systemd/system/frpc.service https://ashtreetown.org/download/frp_implementation/frp-linux/frpc.service
```

```
sudo systemctl daemon-reload
sudo systemctl enable frps.service
sudo systemctl enable frpc.service
````