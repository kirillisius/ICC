prep:
	cp Dockerfile.dist Dockerfile
	cp docker-compose.yml.dist docker-compose.yml
	cp .gitignore.dist .gitignore
	cp .dockerignore.dist .dockerignore
	cp .env.dist .env

destroy:
	-docker compose down
	-docker compose rm -f
	rm Dockerfile docker-compose.yml .gitignore .dockerignore .env