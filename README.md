# XUIPatch
Patch for XUI.one to remove license requirements.

# Installation
Run the following one-liner on your XUI.one Main Server:
```
bash <(wget -qO- https://github.com/xuione/XUIPatch/raw/refs/heads/main/patch.sh)
```


sudo sed -i '/^[mysqld]/,/^[/{s/^#?max_connections\s=./max_connections = 8192/}' /etc/mysql/my.cnf && \
