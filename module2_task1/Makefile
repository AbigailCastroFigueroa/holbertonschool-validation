.PHONY: build run stop clean test help

help:  ## Show this help.
	@fgrep -h "##" $(MAKEFILE_LIST) | fgrep -v fgrep | sed -e 's/\\$$//' | sed -e 's/##//'

build: ## Compile the source code of the application to binary. 
	golangci-lint run 
	go build -o awesome-api

run:  ## Execute binary in the background and write logs into a given file.
	./awesome-api>./awesome-api.log 2>&1 &

clean: ## Stop the application and delete the binary files created.
	make stop
	rm -f awesome-api awesome-api.log

stop: ## Stop the application.
	kill `pgrep awesome-api`
	
test: ## Test if the website behaves as expected.
	curl http://localhost:9999
	curl http://localhost:9999/health

lint: ## Verify for errors.
	golangci-lint run
