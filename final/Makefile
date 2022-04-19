

run: namespace
	kubectl apply -f ./run1 --all

namespace:
	kubectl apply -f ./namespace.yaml

fill-db:
	kubectl apply -f ./run2 --all

stop:
	kubectl delete ns assigment
	