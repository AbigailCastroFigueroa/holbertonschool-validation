.PHONY: build clean post

build: 
	hugo -d dist

clean: 
	rm -rf dist/

post: 
	hugo new posts/$(POST_NAME).md
	sed -i '2s/title: .*/title: "$(POST_TITLE)"/' content/posts/$(POST_NAME).md