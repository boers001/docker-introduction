# Hands on Labs
## Prerequisites


!SUB
### Docker

* For the workshop we use AWS instances.
* Alternatively you can run all handson on your local
  * Linux : Install docker, docker-compose, git and your favourite editor
  * Mac / Windows : Install docker toolbox (includes git and virtual box)


!SUB
### Network
* You should be able to download docker images. Configuring a proxy and setting up docker behind a proxy is not part of this workshop. So we assume you are connected directly to the internet.
* For the AWS setup you should be able to connect via several HTTP ports to your instances as well via SSH.

!SUB
### Linux/Mac Users: How to login to an AWS instance
- Windows users: skip this slide
- We are using a key file (.pem) to access the AWS instances.
'Save link as' [here](key/DOCKER_HANDSON_GRONINGEN.pem) to download the key and save it locally.
- Open an terminal
- Your key must not be publicly viewable for SSH to work.

```
chmod 400 <path>/DOCKER_HANDSON_GRONINGEN.pem
```

- To prevent ssh timeout add ServerAliveInterval=120 as option
to ssh command
- Connect via ssh

```
 ssh -o ServerAliveInterval=120 -i <path>/DOCKER_HANDSON_GRONINGEN.pem ubuntu@<ip-aws-instance>
```

!SUB
### Windows Users: How to login to an AWS instance

- We are using a pem file (.ppk) to access the AWS instances. Click [here](key/DOCKER_HANDSON_GRONINGEN.ppk) to download the key and save it locally.
- Download [putty](http://www.chiark.greenend.org.uk/~sgtatham/putty/download.html)
- Start putty and enter the host ip
- Select `data` on the left hand side under `auto-login username` enter the user `ubuntu`
- Select `SSH`->`Auth` on the left hand side then under `private key for authentication` select the .ppk file we just downloaded.
- To prevent ssh timeout in putty select `connection`. Under "Sending of null packets to keep session active - Seconds between keepalives (0 to turn off)", enter `120` in the text box.
- Go back to the top and connect to your instance.


![logo](images/docker-logo.jpg)

!SUB
### Some guidelines
* You will find the slides here: [http://52.30.86.40/](http://52.30.86.40/)
- Navigation through the slides is easy, just use your arrow keys. Left and right for going to the previous or next section and up and down for previous or next page. The space bar always give you the next page.
- All code blocks unless mentioned are meant to execute by your self.
- Have fun, take your time and feel free to ask questions.
