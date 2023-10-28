# my-ansible-playbooks
My Ansible playbooks

## Setup

```shell script
mkdir -p "${HOME}/.ansible"
cd "${HOME}/.ansible"

rm -rf "my-ansible-playbooks"
git clone "https://github.com/ivasilyev/my-ansible-playbooks.git"

cd "my-ansible-playbooks"

export ANSIBLE_PB_DIR="$(pwd)/playbooks/"
echo "export ANSIBLE_PB_DIR=\"${ANSIBLE_PB_DIR}\"" \
| tee -a  "${HOME}/.bashrc"
# nano "${HOME}/.bashrc"

git pull
```
