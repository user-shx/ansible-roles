# TODO
1. 需要添加操作系统类型验证，如果操作系统不是centos，则退出

# 使用方式
1. 进入ansible工作目录
```bash
cd ~/workspace/ansible
```
2. 使用 ping 模块检测连通性
```bash
ansible -i ./inventory/update_openssh/xxx.ini update_openssh -m ping
```
3. 检查操作系统发行版
```bash
ansible-playbook -i ./inventory/update_openssh/xxx.ini ./playbooks/update_openssh_for_bjtel.yaml -K --tags "check distribution"
```
4. 升级openssh
```bash
ansible-playbook -i ./inventory/update_openssh/xxx.ini ./playbooks/update_openssh_for_bjtel.yaml -K --tags "update openssh"
```
5. 检查sshd的版本
```bash
ansible-playbook -i ./inventory/update_openssh/xxx.ini ./playbooks/update_openssh_for_bjtel.yaml -K --tags "check version"
```