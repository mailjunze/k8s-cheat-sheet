# k8s-cheat-sheet
download : https://kubernetes.io/docs/tasks/tools/
## bash
echo "source <(kubectl completion bash)" >> ~/.bashrc

echo "alias k=kubectl" >> ~/.bashrc

complete -o default -F __start_kubectl k

source ~/.bashrc
