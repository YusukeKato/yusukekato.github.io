# Install nginx
- WSL2/Ubuntu 24.04 LTS

```sh
sudo apt install curl gnupg2 ca-certificates lsb-release ubuntu-keyring
curl https://nginx.org/keys/nginx_signing.key | gpg --dearmor | sudo tee /usr/share/keyrings/nginx-archive-keyring.gpg >/dev/null
gpg --dry-run --quiet --no-keyring --import --import-options import-show /usr/share/keyrings/nginx-archive-keyring.gpg
echo "deb [signed-by=/usr/share/keyrings/nginx-archive-keyring.gpg] http://nginx.org/packages/ubuntu `lsb_release -cs` nginx" | sudo tee /etc/apt/sources.list.d/nginx.list
echo -e "Package: *\nPin: origin nginx.org\nPin: release o=nginx\nPin-Priority: 900\n" | sudo tee /etc/apt/preferences.d/99nginx
sudo apt update
sudo apt install nginx
```

# Start nginx
```sh
sudo systemctl start nginx
sudo systemctl enable nginx
```

# Setup files
```
/etc/nginx/conf.d/default.conf
/etc/nginx/nginx.conf
```

# Access
[http://localhost/](http://localhost/)

[参考](https://nginx.org/en/linux_packages.html#Ubuntu)

![](../../images/BlueTreeIcon_200x200.jpg)

[YKpages Home Page](https://yusukekato.github.io/)
