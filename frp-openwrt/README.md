## frp working location
`/opt/frp`

## Download frp
`wget https://ashtreetown.org/resource/software/frp/latest/frp_linux_amd64.tar.gz`
`wget https://ashtreetown.org/resource/software/frp/latest/frp_linux_arm64.tar.gz`

## frp server location
```
wget -O /etc/init.d/frpc https://ashtreetown.org/download/frp_implementation/frp-openwrt/frpc
chmod +x /etc/init.d/frpc
/etc/init.d/frpc enable
```