# caffe-ansible
Minimal caffe environment build by ansible

```bash
git clone git clone https://github.com/ganow/caffe-ansible.git

vagrant up
vagrant ssh -- -L 8888:localhost:8888


sudo apt-get update
sudo apt-get install python-pip
sudo pip install ansible


cd /vagrant
ansible-playbook playbook.yml -i localhost


ipython notebook --no-browser
```
