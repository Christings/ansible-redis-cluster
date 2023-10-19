# ansible-redis-cluster
通过ansible搭建 Redis Cluster 集群环境(Docker)

# 安装ansible
    apt-get install ansible  
    yum install ansible

# 建立机器互信机制
    ssh-keygen -t rsa
    ssh-copy-id -i ~/.ssh/id_rsa.pub username@ip1
    ssh-copy-id -i ~/.ssh/id_rsa.pub username@ip2

## 执行命令
ansible-playbook -i hosts_install -e @vars_install.json setup.yml 

# 备注
去掉sudo，否则执行时会不断进行连接
