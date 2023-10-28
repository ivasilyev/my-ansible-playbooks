# my-ansible-playbooks
My Ansible playbooks

## Setup

```shell script
mkdir -p "${HOME}/.ansible"

git clone "https://github.com/ivasilyev/my-ansible-playbooks.git"
cd "my-ansible-playbooks"
cd "${HOME}/.ansible/my-ansible-playbooks"

export ANSIBLE_PB_DIR="$(pwd)"
echo "export ANSIBLE_PB_DIR=\"${ANSIBLE_PB_DIR}\"" \
| tee -a  "${HOME}/.bashrc"

git pull
```
