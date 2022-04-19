

run:
	kubectl apply -f ./run1 --all

fill-db:
	kubectl apply -f ./run2 --all

stop:
	kubectl delete deploy back data front
	kubectl delete pod data-script-pod
	kubectl delete secret data-secret back-secret data-script-secret
	kubectl delete service back data front

clean:
	kubectl delete pvc claim
	kubectl delete sc sc  