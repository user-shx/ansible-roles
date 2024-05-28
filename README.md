# ansible-roles
记录一些ansible安装软件的示例。

# 工作目录结构
```
ansible/
├── ansible.cfg            # 配置文件
├── files                  # 存放一些文件，上传或下载的位置
├── inventory              # 存放清单配置
│   ├── production         # 生产环境的信息
│   │   ├── group_vars
│   │   ├── hosts
│   │   └── host_vars
│   └── staging            # 测试环境的信息
│       ├── group_vars
│       ├── hosts
│       └── host_vars
├── logs                   # ad-hoc或playbook执行结果的日志存放位置
├── playbooks              # playbook 存放位置
└── role                   # 角色存放位置
```