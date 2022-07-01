project=web3
now=$(shell date +'%d-%m-%Y')

SHELL=/bin/zsh
.SHELLFLAGS = -e -o pipefail -c

infra-up:
	docker-compose -f ./docker-compose.yaml -p $(project) up -d

infra-build:
	docker-compose -f ./docker-compose.yaml -p $(project) build

infra-down:
	docker-compose -f ./docker-compose.yaml -p $(project) down --remove-orphans

infra-logs:
	docker-compose -f ./docker-compose.yaml -p $(project) logs -t -f

