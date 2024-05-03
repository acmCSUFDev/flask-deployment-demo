# Flask Deployment Demo

> A premade Flask template for deploying!

## About Flask

Flask is a web framework that allows you to create web applications using the
Python programming language. In simple terms, Flask provides you with tools and
features that make it easier to build web applications.

A web application is a software program that runs in a web browser. For
example, when you use Facebook or Instagram, you're using a web application.

Flask makes it easy to create a web application by providing a set of functions
and tools that help you:

- Define the structure of your application, such as the different pages or URLs users can access.
- Define the behavior of your application, such as what happens when a user clicks a button or fills out a form.
- Store and retrieve data, such as user information or images.

## How to Deploy

1. Install Python 3 or later: `sudo apt install python3`
2. Enter root user to make system-wide changes: `sudo su`
3. Clone this repository: `git clone https://github.com/acmCSUFDev/flask-deployment-demo /opt/flask-deployment-demo`
4. Go to the directory: `cd /opt/flask-deployment-demo`
5. Load Python virtualenv and install dependencies: `. ./init`
6. Install the systemd service: `ln -s /opt/flask-deployment-demo/flask-deployment-demo.service /etc/systemd/system/flask-deployment-demo.service`
7. Reload systemd: `systemctl daemon-reload`
8. Start the service now and on startup: `systemctl enable --now flask-deployment-demo`
9. Check the status of the service: `systemctl status flask-deployment-demo`
10. Check the logs: `journalctl -u flask-deployment-demo`
