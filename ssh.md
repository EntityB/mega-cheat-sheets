### ssh keys types
```sh
ssh-keygen -t rsa -b 4096
ssh-keygen -t dsa
ssh-keygen -t ecdsa -b 521
ssh-keygen -t ed25519
```

### set permisions (mandatory)
```sh
chmod 600 ~/.ssh/<ssh_key>
chmod 600 ~/.ssh/<ssh_key>.pub
```

### setting multiple ssh keys (for git):
```sh
# create a new ssh key with different name and then:
touch ~/.ssh/config
chmod 600 ~/.ssh/config
vi config
```
config file content
```sh
# config file content

# server that will use different then default ssh key
Host bitbucket2
        HostName bitbucket.org
        IdentityFile ~/.ssh/<ssh_key>
```
clone with git
```sh
git clone git@bitbucket2:<some path>/<some project>.git
```
