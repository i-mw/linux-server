# Linux Server Deployment

Linux server deployment is the last project at Udacity's full-stack nanodegree.

The goal of the project is to deploy a project to a linux server and to protect the server.

## Instructions to access the server
Use bash's `ssh` command line to access the remote machine according to this syntax:
```
ssh <user_name>@<ip_address> -p <port> -i <private_key>
```
- user_name: `grader`
- ip_address : `18.184.94.109`
- port: `2200`
- private_key: messaged privately

- Url of the app: `http://18.184.94.109.xip.io`

N.b. to view the app in the browser, use the url and not the ip, as Google's requires a hostname for Oauth to work on the website.

## Installed Software
- Apache2
- SQLite3
- mod-wsgi for python3
- pip3
- finger


## Third Party Resources
- flask
- requests
- sqlalchemy
- oauth2client
- Google's OAuth

## Configuration Changes made
- Set and enable the firewall to allow only connections over 80, 2200 and 123 ports
- create grader user
- give him sudo access
- restrict access to ssh keys
- configure timezone
- install and update required software
- deploy the project's code
- connect wsgi file to project's code
- change all project's files owner and group to www-data and no one else has permissions.