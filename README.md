# cka-docs-practice
This repo is created for CKA Training and all Documents and practice files.

nginx-sample.yaml

1. Create a basic manifest file to deploy nginx pod.
2. Create a Service file for external access use NodePort.
3. Label the node in which you want to Schedule the Pod.
Command:
kubectl label node nodename <key>:<value>
4. Verify using kubectl describe node nodename | grep -i labels
5. Now use nodeAffinity to Schedule to pod. Node Affinity has the advance featured for Scheduling the pod in a specific node.
For Basic feature we can directly use nodeSelector or nodeName.
6. For Advance Practice we have use nodeAffinity.
7. Kubectl apply both the manifest file and then try to access the nginx from browser using clusterIP and nodePort.
