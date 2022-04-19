

run:
	kubectl apply -f ./all-services/
	kubectl apply -f ./storage-class/

fill-db:
	kubectl apply -f ./data-script

stop:
	kubectl delete -f ./all-services/

clean:
	kubectl delete -f ./storage-class/
	