# vagrant

通过packer工具制作box文件(参考[git](https://github.com/boxcutter/centos.git))

导入自制的box(centos7.4)`vagrant box add centos7.4`

根据需求修改vagrantfile文件里主机创建数量NODENUM=?值

创建主机`vagrant up`(因vagratfile文件已存在不需要执行初始化vagrant init操作)

