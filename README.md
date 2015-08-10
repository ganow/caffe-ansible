# caffe-ansible
Minimal caffe environment build by ansible

## How to use

Clone this repository into your project directory.

```bash
git clone https://github.com/ganow/caffe-ansible.git /path/to/caffe-ansible
```

Start VM and access to it.

```bash
cd /path/to/caffe-ansible
vagrant up
vagrant ssh -- -L 8888:localhost:8888
```

Install ansible to the VM.

```bash
sudo apt-get update
sudo apt-get install python-pip
sudo pip install ansible
```

Build Caffe environments with ansible

```bash
cd /vagrant
ansible-playbook playbook.yml -i localhost
```

Boot up IPython Notebook.

```bash
cd ~/caffe
ipython notebook --no-browser
```

# Requirements

- Virtualbox
- vagrant
