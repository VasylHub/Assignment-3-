

run:
	kubectl apply -f ./all-services/
	kubectl apply -f ./storage-class/

fill-db:
	kubectl apply -f ./data-script

stop:
	kubectl delete -f ./all-services/
	kubectl delete -f ./data-script

clean: stop
	kubectl delete -f ./storage-class/
	