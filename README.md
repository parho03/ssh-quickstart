## SSH Key Setup Instructions

# 1. Generate a new RSA SSH key in PEM format
ssh-keygen -t rsa -b 4096 -m PEM -f ~/.ssh/<key_name>

# 2. List your SSH keys to verify
ls ~/.ssh

# 3. Copy the public key to the remote server
ssh-copy-id -i ~/.ssh/key_name.pub user@ip-address

# 4. Test SSH login
ssh -i ~/.ssh/key_name user@ip-address
