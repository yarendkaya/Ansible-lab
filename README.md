# Automated Nginx Deployment with Ansible & Vagrant

This project demonstrates a local **Infrastructure as Code (IaC)** lab environment. It uses **Vagrant** to provision a multi-machine Ubuntu environment and **Ansible** to automate the configuration and deployment of the **Nginx** web server.

## 🏗 Project Architecture

The lab consists of two virtual machines running Ubuntu 18.04 (Bionic):

| Machine Name   | IP Address      | Role |
| :---           | :---            | :--- |
| **Control Node** | `192.168.56.10` | The Ansible controller machine. Runs the playbooks. |
| **Managed Node** | `192.168.56.20` | The target server where Nginx is installed. |

## 🚀 Technologies Used

* **Vagrant:** For reproducible development environments.
* **VirtualBox:** As the virtualization provider.
* **Ansible:** For configuration management and application deployment.
* **Nginx:** High-performance web server.

## 📂 Project Structure

* `Vagrantfile`: Defines the VM configuration (CPU, Memory, Network, IPs).
* `playbook.yml`: The Ansible playbook that installs and starts Nginx.
* `hosts`: The Ansible inventory file defining the target servers and connection settings.

## 🛠️ Setup & Installation

Follow these steps to get the environment running:

### 1. Clone the Repository
```bash
git clone [https://github.com/yarendkaya/Ansible-lab.git](https://github.com/yarendkaya/Ansible-lab.git)
cd Ansible-lab

Harika, işte projen için hazırladığım profesyonel ve kapsamlı İngilizce README.md dosyası.

Bunu kopyalayıp GitHub'daki README.md dosyanın içine yapıştırabilirsin.

Markdown

# Automated Nginx Deployment with Ansible & Vagrant

This project demonstrates a local **Infrastructure as Code (IaC)** lab environment. It uses **Vagrant** to provision a multi-machine Ubuntu environment and **Ansible** to automate the configuration and deployment of the **Nginx** web server.

## 🏗 Project Architecture

The lab consists of two virtual machines running Ubuntu 18.04 (Bionic):

| Machine Name   | IP Address      | Role |
| :---           | :---            | :--- |
| **Control Node** | `192.168.56.10` | The Ansible controller machine. Runs the playbooks. |
| **Managed Node** | `192.168.56.20` | The target server where Nginx is installed. |

## 🚀 Technologies Used

* **Vagrant:** For reproducible development environments.
* **VirtualBox:** As the virtualization provider.
* **Ansible:** For configuration management and application deployment.
* **Nginx:** High-performance web server.

## 📂 Project Structure

* `Vagrantfile`: Defines the VM configuration (CPU, Memory, Network, IPs).
* `playbook.yml`: The Ansible playbook that installs and starts Nginx.
* `hosts`: The Ansible inventory file defining the target servers and connection settings.

## 🛠️ Setup & Installation

Follow these steps to get the environment running:

### 1. Clone the Repository
```bash
git clone [https://github.com/yarendkaya/Ansible-lab.git](https://github.com/yarendkaya/Ansible-lab.git)
cd Ansible-lab
### 2. Provision the Virtual Machines
vagrant up
### 3. Connect to the Control Node
vagrant ssh control_node
### 4. Run the Ansible Playbook
ansible-playbook -i /vagrant/hosts /vagrant/playbook.yml

Open your browser and visit: https://www.google.com/search?q=http://192.168.56.20

You should see the "Welcome to nginx!" default page.
