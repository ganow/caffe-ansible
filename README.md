# caffe-ansible
Minimal caffe environment build by ansible

```bash
vagrant box add ubuntu14.04 https://cloud-images.ubuntu.com/vagrant/trusty/current/trusty-server-cloudimg-amd64-vagrant-disk1.box
git clone caffe-ansible

vagrant up
vagrant ssh -- -L 8888:localhost:8888


sudo apt-get update
sudo apt-get install python-pip
sudo pip install ansible


cd /vagrant
ansible-playbook playbook.yml -i localhost


ipython notebook --no-browser
```
