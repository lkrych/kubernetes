kube-start:
	kubectl apply -f k8s/deployment.yaml
	kubectl apply -f k8s/service.yaml

kube-map:
	kubectl port-forward service/demo 9999:8888

kube-clean:
	kubectl delete -f k8s/

kube-pod-ls:
	kubectl get pods --selector app=demo

kube-deployments-ls:
	kubectl get deployments

kube-deployments-info:
	kubectl describe deployments/demo

kube-nodes-ls:
	kubectl get nodes
