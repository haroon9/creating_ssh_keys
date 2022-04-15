# Creating_ssh_keys

## Generate a new key using
```
ssh-keygen -t ed25519 -C "your_email@example.com"
```

## start ssh-agent in the key background
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
 
 Now your git clone using ssh will work.
