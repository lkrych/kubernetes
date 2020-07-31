build:
	docker image build -t kubehello .

start:
	docker container run -p 9999:8888 kubehello

kube-start:
	kubectl run demo --image=ellk/kubehello --port=9999 --labels app=demo

kube-map:	
	kubectl port-forward deploy/demo 9999:8888
	
kube-clean:
	kubectl delete all --selector app=demo

kube-pod-ls:
	kubectl get pods --selector app=demo

kube-deployments-ls:
	kubectl get deployments

kube-describe:
	kubectl describe deployments/demo
