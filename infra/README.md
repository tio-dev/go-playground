# minio console

```bash
❯ wget https://dl.min.io/client/mc/release/linux-amd64/mc
❯ chmod +x mc
❯ sudo cp ./mc /usr/local/bin
```

```bash 
❯ mc config host add boafe http://127.0.0.1:9007 minioweb3 minioweb3 
❯ mc admin user add boafe console minioconsole 
❯ mc admin policy add boafe consoleAdmin consoleAdmin.json
❯ mc admin policy set boafe consoleAdmin user=console
```
