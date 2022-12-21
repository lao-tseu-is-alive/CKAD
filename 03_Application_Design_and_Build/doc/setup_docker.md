## Commands to setup Machine for Docker Environment
Commands to Install Docker on Linux(Ubuntu) Machine
Please execute the all commands in sequence as they given.

1. sudo apt-get update

2. sudo apt-get install \
   lsb-release \
   ca-certificates \
   gnupg \
   ca-certificates

3. curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg

4. echo \
   "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu \
   $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null

5. sudo apt-get update

6. sudo apt-get install docker-ce docker-ce-cli containerd.io

7. docker version

8. sudo docker run hello-world

## More info : 
https://docs.docker.com/engine/install/ubuntu/