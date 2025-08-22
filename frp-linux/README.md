/usr/bin/frps
/usr/bin/frpc

/etc/frp/frps.toml
/etc/frp/frpc.toml

sudo useradd -r -s /bin/false frp
sudo chown -R frp:frp /etc/frp

cp frps.service /usr/lib/systemd/system/frps.service