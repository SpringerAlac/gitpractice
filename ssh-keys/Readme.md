
This is how you can use the Linux Shell (also on Git Bash) to generate public and private keys. 

```sh
ssh-keygen -t rsa
ssh-keygen -t ed25519
cat /home/codespace/.ssh/id_ed25519.pub
```

Get the public key (end with .pub) and put that output in GitHub setting where you can store SSH keys.