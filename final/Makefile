

run:
	kubectl apply -f back-deployment.yaml
	kubectl apply -f back-secret.yaml
	kubectl apply -f back-service.yaml
	kubectl apply -f data-deployment.yaml
	kubectl apply -f data-secret.yaml
	kubectl apply -f data-service.yaml
	kubectl apply -f front-deployment.yaml
	kubectl apply -f front-service.yaml
	kubectl apply -f sc.yaml

fill-db:
	kubectl apply -f data-script-pod.yaml
	kubectl apply -f data-script-secret.yaml

stop:
	kubectl delete deploy back data front
	kubectl delete pod data-script-pod
	kubectl delete secret data-secret back-secret data-script-secret
	kubectl delete service back data front

clean:
	kubectl delete pvc claim
	kubectl delete sc sc 