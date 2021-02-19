# awx-tower
Ansible playbook for awx installation

Before runnig the playbook do the following


Step One
sudo su
rpm -ivh http://rpmfind.net/linux/epel/7/x86_64/Packages/e/epel-release-7-13.noarch.rpm
yum install ansible -y
ansible --version





yum-config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo

cd /etc/yum.repo.d
vi docker-ce.repo 

UPDATE The first line to match below


name=Docker CE Stable - $basearch
baseurl=https://download.docker.com/linux/centos/7/$basearch/stable
enabled=1
gpgcheck=1
gpgkey=https://download.docker.com/linux/centos/gpg
