# Hugo Website
In this project we will learn how to build a website with the hugo framework.

## Prerequisites
To fullfill this project you would need a computer with the following tools and programs installed based on your operating system:
- [GoHugo](https://gohugo.io/installation/) v0.84.0
- [Git] (https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
- GNU Make 
- An HTML5-compliant web browser (Firefox, Chrome, Opera, Safari, Edge, etc.)

## Lifecycle
In this project we use the following commands using a makefile to construct the website.
- build: Generate the website from the markdown and configuration files in a given directory.
- clean: Clean all the content from the directory where the website was generated.
- post: Create a new blog post whose filename and title come from enviroment variables.
- help: Show the makefile targets and the description of what the task that perform each one.
