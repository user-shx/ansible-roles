# fixed
## 2024-04-30
1. 修改`config yum`的内容，只备份 CentOS-http.repo，其他镜像文件不动

## 2024-04-29
1. 将升级openssh的task添加 `update openssh` tag.
2. 新增`check distribution` tag, 检查操作系统发行版

## 2024-04-15 
1. 新增 config yum 的tags
支持配置yun源，指定 --tags "config yum"
2. 重新处理 /etc/init.d/sshd 文件的备份，如果没有该文件则不进行备份
3. 新增`check version`的 tags，检查sshd版本