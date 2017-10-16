CLI for Mycloudapp
## About MyCloudApps
Deploy your apps to the cloud quickly and easily with MyCloudApp. 
Get up and running in a few minutes.

Deploy everything from the command line, its so easy.

## Highlights

- Create an account from the command line
- Deploy or Delete a Mongodb Database in seconds!!

## Install

```console
$ npm install mycloudapp
```


## Usage
### Create an Account

```console
$ mycloudapp user register
```

You will be prompted to enter your email and a password.

Mycloudapp will return a `token` which you will use for authentication.

### Deploy a Mongodb Database
```console
$ mycloudapp mongodb deploy <name> <port>
```
where `name` is the name of your Mongodb Database and `port` is the port number.

Once created, the server details will be returned and you can connect to it and get going.

``Its that easy!!.``

## Other Commands
### List active Mongodb Apps
```console
$ mycloudapp list apps mongodb
```
You will see a list of Mongodb apps that are active. The `app id` will also be displayed. This can be used to delete the database.

### Delete a Mongodb Database
```console
$ mycloudapp mongodb delete <id>
```
### Get User Token
```console
$ mycloudapp user token
```
You will need to enter you registered email and password. Once vaildated, your token will be displayed.

### List Current Logged In User
```console
$ mycloudapp user list
```
### Change the Current Logged In User 
```console
$ mycloudapp user set <email> <token>
```
