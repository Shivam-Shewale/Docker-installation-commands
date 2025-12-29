# Docker Installation 

# Update the system 
       apt update -y 

# Install required packages  
      sudo apt install -y ca-certificates curl gnupg lsb-release

# Add Docker’s official GPG key 
       sudo mkdir -p /etc/apt/keyrings
       curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg

 # Add Docker repository 
        echo \
        "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.gpg] \
         https://download.docker.com/linux/ubuntu \
        $(lsb_release -cs) stable" | \
        sudo tee /etc/apt/sources.list.d/docker.list > /dev/null

# Update package index again 
         apt update -y

# Now Install Docker engine 
         sudo apt install -y docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin

# Verify if docker installed 
         docker --version

# Start and Enable docker and check status 
         systemctl start docker
         systemctl enable docker
         systemctl status docker    
