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
```
ansible prod-* -m command -a "chage -l root" -b --become-method sudo
time ansible all -m shell -a 'chage -d `date -d "$(($RANDOM%60)) days ago" +%Y-%m-%d` root'
sudo chage -m 0 -M 99999 -I -1 -E -1 root
```
