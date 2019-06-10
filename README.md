# ansible-playbook

### common nginx php nodejs mysql redis

```
mv group_vars/all_EXAMPLES group_vars/all
vi group_vars/all
```
```
# install
yum install ansible

# test
ansible-playbook hello.yml -i ~/hosts

# run
ansible-playbook site.yml -i ~/hosts

```
