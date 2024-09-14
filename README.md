# DNS-kali
### Enable disable resolved service where we can utilize this service to manage dns locally

status check resolved
```sudo systemctl status systemd-resolved.service```

start
```sudo systemctl start systemd-resolved.service```

stop
```sudo systemctl stop systemd-resolved.service```

If you use this service it runs dns queires locally(Its mostly used in AD pentesting to configure dns)
![image](https://github.com/user-attachments/assets/f79ebfcf-ff5b-4816-b728-65b6d5acdbed)

Configure dns server with resolvectl command - resolved.service cli tool
```resolvectl dns interface dnsip```
![image](https://github.com/user-attachments/assets/4e74b7c9-5aa4-46d8-b486-9e12fdd857a4)



# Enable default DNS server on kali
Edit /etc/resolv.conf and a name server entry with google dns servers

```nano /etc/resolv.conf
nameserver 8.8.8.8```
now its uses google to resolve domains
![image](https://github.com/user-attachments/assets/8b9105c8-ed44-44f4-b677-de5eb5fce6eb)

