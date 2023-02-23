
DOCKER_COMPOSE := docker compose
DOCKER_COMPOSE_FILE := docker-compose.yml

.PHONY: up
up:
	$(DOCKER_COMPOSE) -f $(DOCKER_COMPOSE_FILE) up -d

.PHONY: down
down:
	$(DOCKER_COMPOSE) -f $(DOCKER_COMPOSE_FILE) down

.PHONY: clean
clean:
	$(DOCKER_COMPOSE) -f $(DOCKER_COMPOSE_FILE) down -v
run-nginx:
	 @amazon-linux-extras install nginx1 -y
	@systemctl enable nginx
	@systemctl start nginx
	@systemctl status nginx
	@echo 'Testing Nginx local webpage'
	@curl localhost:8080
run-docker:
	@yum install docker -y
	@systemctl start docker
	@systemctl enable docker
	@echo 'Testing Docker status'
	@systemctl status docker
docker-build:
	@docker build -t Dockerfile.dist:latest .
	@@docker run -p 80:80 -d Dockerfile.dist:latest
