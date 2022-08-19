# install dev environment for new computer


### Install sudo and git if needed
```
apt-get update && apt-get install -y git sudo
```

### If no user was created
```
useradd -m -s /bin/bash -G sudo eliag && echo "<username>:<password>" | chpasswd && su <username> && cd ~
```

### Clone and install ansible
```
git clone https://github.com/EliaGuarnieri/ansible.git && cd ./ansible && ./install
```

### Run ansible

```
./ansible-run
```

# TODOS
- [] Add zsh plugins
- [] Add variable to use with different user
- [] Cloning personal repositories
- [] Add pwsh script for portability
- [] Check if ansible allow different approch for ssh key