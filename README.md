# Automated-VM-deployment
The following Vagrant file allows and automated deployment of 4 VMs with optional operating system. The following code can be Scalable for user personal project.
# Vagrant Multi-OS Cluster

This project sets up a cluster of 4 virtual machines with Vagrant and VirtualBox, allowing users to choose between Ubuntu 22.04 LTS, CentOS 8, or Debian 10.

## Usage
### Requirements
- Vagrant
- VirtualBox

### Steps
1. Clone the repository:
    ```bash
    git clone https://github.com/username/vagrant-multi-os-cluster.git
    cd vagrant-multi-os-cluster
    ```
2. Navigate to the project directory:
    ```bash
    cd vagrant-multi-os-cluster
    ```
3. Start the VMs:
    ```bash
    vagrant up
    ```
4. Follow the prompts to select your desired OS:
    ```plaintext
    1. Ubuntu 22.04 LTS 
    2. CentOS 8
    3. Debian 10
    ```
5. Create a new username and password when prompted.
6. Access the VMs:
    ```bash
    vagrant ssh node1
    vagrant ssh node2
    vagrant ssh node3
    vagrant ssh node4
    ```
7. Tear down the VMs when done:
    ```bash
    vagrant destroy -f
    ```
### Configuration
- `NUM_NODES`: Number of VMs to be created (default: 4).
- `vm.box`: User-selected operating system.
- Each VM is assigned a private IP starting from `192.168.56.101`.
- Each VM is allocated 512MB of RAM and a 20GB storage disk.

