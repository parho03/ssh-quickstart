## SSH Key Setup Instructions

# 1. Generate a new RSA SSH key in PEM format
```bash
ssh-keygen -t rsa -b 4096 -m PEM -f ~/.ssh/<key_name>
```
# 2. List your SSH keys to verify
```bash
ls ~/.ssh
```

# 3. Copy the public key to the remote server
```bash
ssh-copy-id -i ~/.ssh/key_name.pub user@ip-address
```

# 4. Test SSH login
```bash
ssh -i ~/.ssh/key_name user@ip-address
```
