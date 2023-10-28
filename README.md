# my-ansible-playbooks
My Ansible playbooks

## Setup

```shell script
mkdir -p "${HOME}/.ansible"

export ANSIBLE_PB_DIR="${HOME}/.ansible/my-ansible-playbooks/"
echo "export ANSIBLE_PB_DIR=\"${ANSIBLE_PB_DIR}\"" \
| tee -a  "${HOME}/.bashrc"
# nano "${HOME}/.bashrc"

rm -rf "${ANSIBLE_PB_DIR}"

git clone \
    "https://github.com/ivasilyev/my-ansible-playbooks.git" \
    "${ANSIBLE_PB_DIR}"

cd "${ANSIBLE_PB_DIR}"

git pull
```
