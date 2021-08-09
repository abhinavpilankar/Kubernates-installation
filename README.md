# Kubernates-installation...


curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"

sudo install -o root -g root -m 0755 kubectl /usr/local/bin/kubectl

if you do not have root access on the target system, you can still install kubectl to the ~/.local/bin directory:

mkdir -p ~/.local/bin/kubectl
mv ./kubectl ~/.local/bin/kubectl
and then add ~/.local/bin/kubectl to $PATH

kubectl version --client

