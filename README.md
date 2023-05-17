# HA-proxy-setup
HA-proxy-setup with Vagrant and Ansible

![Screen Shot 2023-05-17 at 5 41 21 PM](https://github.com/ron8cr/HA-proxy-setup/assets/124076577/4588706f-cfeb-4fe9-aec9-1b2bd8885e69)

# HAProxy Proxy to Google.com
This project sets up a High Available HAProxy setup acting as a proxy to Google.com. It utilizes Vagrant, VirtualBox, CentOS, Ansible, HAProxy, and KeepAlived. The setup includes master-slave high-availability mode and proxying requests from a custom domain to Google.com.

## Project Structure
- Vagrantfile: Vagrant configuration file for provisioning VMs.
- ansible/: Ansible playbook and template files.
- ansible/haproxy-master.yml: Ansible playbook for configuring the HAProxy master instance.
- ansible/haproxy-slave.yml: Ansible playbook for configuring the HAProxy slave instance.
- ansible/haproxy-virtualip.yml: Ansible playbook for configuring the HAProxy virtual IP instance.
- ansible/templates/: Directory containing template files for HAProxy and Keepalived configurations.

## Prerequisites
- Vagrant: Installation guide
- VirtualBox: Installation guide

## Setup Instructions
1. Clone the repository:
```
git clone https://github.com/your-username/haproxy-proxy.git
cd haproxy-proxy
```
2. Start the Vagrant environment:
```
vagrant up
```
3. Wait for the VMs to be provisioned and configured.

4. Access the HAProxy instance by opening a browser and navigating to https://my-google.com.

## Customization
- To modify the HAProxy configuration, edit the ansible/templates/haproxy.cfg.j2 template file.
- To modify the Keepalived configuration, edit the ansible/templates/keepalived.conf.j2 template file.




