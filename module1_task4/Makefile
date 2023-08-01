.PHONY: build clean post help

help:  ## Show this help.
	@fgrep -h "##" $(MAKEFILE_LIST) | fgrep -v fgrep | sed -e 's/\\$$//' | sed -e 's/##//'

build: ## Generate the website from the markdown and configuration files in a given directory. 
	hugo -d dist

clean: ## Clean all the content from the directory where the website was generated.
	rm -rf dist/

post:  ## Create a new blog post whose filename and title come from enviroment variables.
	hugo new posts/$(POST_NAME).md
	sed -i '2s/title: .*/title: "$(POST_TITLE)"/' content/posts/$(POST_NAME).md

