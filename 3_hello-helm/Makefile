helm-start:
	kubectl apply -f helm-auth.yaml
	helm install demo ./k8s/demo

helm-ls:
	helm list

helm-clean:
	helm uninstall demo

kube-clean:
	kubectl delete all --selector app=demo
