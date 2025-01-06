# **<span style="color:green">FEWA IT CONSULTING</span>**

### **<span style="color:green">Contact Information</span>**
- **Phone:** +1 (204) 590-6022
- **Website:** [FEWA IT Consulting](https://fewaitconsulting.cloud/)
- **Email:** [olajide.usman@fewaitconsulting.cloud](mailto:oladevopsdock@gmail.com)

## **Github and Visual Studio Code Integration for Developers**

### **Prerequisites**
- An Github account
- Visual Studio Code on local machine
  
### **Step 1: Generate SSH Keys from Vscode**

Update the package list to ensure all packages are up-to-date.

```sh
# Update the package list
sudo apt update -y
```

### **Step 2: Install Docker**

Install Docker from the Ubuntu repositories.

```sh
# Install Docker
sudo apt install docker.io -y
```

### **Step 3: Start Docker Service**

Start the Docker service and verify the installation.

```sh
# Start Docker service
sudo service docker start

# Display Docker information
sudo docker info
```

### **Step 4: Set Hostname**

Set the hostname to 'docker' for the EC2 instance.

```sh
# Set the hostname to 'docker'
sudo hostnamectl set-hostname docker
```

### **Step 5: Add User to Docker Group**

Add the current user to the Docker group to run Docker commands without sudo.

```sh
# Add the 'ubuntu' user to the Docker group
sudo usermod -aG docker ubuntu

# Switch to the 'ubuntu' user
sudo su - ubuntu
```

### **Step 6: Verify Docker Installation**

Exit the current SSH session, log in again, and verify Docker installation by running a simple Docker command.

```sh
# Exit the current SSH terminal
exit

# SSH login again and run the following command to verify Docker installation
docker ps
```
