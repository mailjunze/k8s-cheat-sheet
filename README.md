# k8s-cheat-sheet
download : https://kubernetes.io/docs/tasks/tools/
## bash
echo "source <(kubectl completion bash)" >> ~/.bashrc

echo "alias k=kubectl" >> ~/.bashrc

complete -o default -F __start_kubectl k

source ~/.bashrc

k create deployment nginx-project --image=nginx
k expose deployment nginx-project --type=NodePort --port=80 --name=nginx-service

k get configmaps -n kube-system
