# Creating_ssh_keys

## Generate a new key using
```
ssh-keygen -t ed25519 -C "your_email@example.com"
```

## copy the key
```
clip < ~/.ssh/id_ed25519.pub
```

## start ssh-agent in the background using
 ```
 eval "$(ssh-agent -s)"
 ```
 
 ## add the newly generated private key to ssh-agent
 ```
 ssh-add ~/.ssh/id_ed25519
 ```
 
 ## add the key inside version control
 Now add your key to the version control whether bibucket, Github or Gitlab etc and then clone your repository with ssh.
