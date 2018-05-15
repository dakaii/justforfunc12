build:
	GOOS=linux go build -o app
	docker build -t gcr.io/cobalt-balancer-116014/say .
	rm -f app

push:
	gcloud auth configure-docker
	docker push gcr.io/cobalt-balancer-116014/say
