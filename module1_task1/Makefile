.PHONY: build clean post

build: 
	hugo -v

clean: 
	rm -rf dist

post: 
	hugo new posts/$(POST_NAME).md
	echo 'title = "$(POST_TITLE)"' >> $(POST_NAME).md