# Argo-Demo
Demo with Argo CD

Need Kubernates installed

### Install Argo
# Mac
Available via brew

brew install argoproj/tap/argo
And via curl

# Download the binary
curl -sLO https://github.com/argoproj/argo/releases/download/v2.6.4/argo-darwin-amd64

# Make binary executable
chmod +x argo-darwin-amd64

# Move binary to path
mv ./argo-darwin-amd64 /usr/local/bin/argo

# Test installation
argo version
# Linux
Available via curl

# Download the binary
curl -sLO https://github.com/argoproj/argo/releases/download/v2.6.4/argo-linux-amd64

# Make binary executable
chmod +x argo-linux-amd64

# Move binary to path
mv ./argo-linux-amd64 /usr/local/bin/argo

# Test installation
argo version
Argo Controller
kubectl create namespace argo
kubectl apply -n argo -f https://raw.githubusercontent.com/argoproj/argo/v2.6.4/manifests/install.y

Blog post with more details over at https://blog.baeke.info/2019/12/25/giving-argo-cd-a-spin/
