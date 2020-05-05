# UDAGRAM

### Setup

Steps to store the environment variables in .bash_profile file
* Create (if not exists) a .profile file in ~ or $HOME directory to contain the user-specific variables. Follow the below steps:
* In the ~ directory, run echo $PATH. Copy the output.
* Create a new .profile file using touch .bash_profile.
* Open it up for editing using any editor. Add the copied $PATH variable value, for example:
    `export PATH=$PATH:/usr/local/mysql/bin/`

* Add the value for other variables specific for you:
  ```
  export POSTGRESS_USERNAME=myusername;
  export POSTGRES_PASSWORD=mypassword;
  export POSTGRES_DATABASE=postgres;
  export POSTGRES_HOST=udagramdemo.abc4def.us-east-2.rds.amazonaws.com;
  export AWS_REGION=us-east-2;
  export AWS_PROFILE=default;
  export AWS_MEDIA_BUCKET=udagramdemo;
  export JWT_SECRET=helloworld;
 
Change the values of the above mentioned variables as applicable for you.
  
 ### Prerequisites
  Before we get started, confirm that you have installed NodeJs, npm and Ionic Framework by checking the versions:

```
node --version
npm --version
ionic --version. 
  ```


If you get a not found message, install the required item:



[Ionic CLI](https://ionicframework.com/docs/intro/cli) if you don't already have it installed
[Nodejs and npm](https://nodejs.org/en/download/)

### Run with Docker
*  `cd docker/`
*  `docker-compose -f docker-compose-build.yaml build --parallel`
* `docker-compose up`

### AWS-deployed url
[server](http://aaba3fe2fc06d4d3ea32dd72e943cfce-1443023894.ap-south-1.elb.amazonaws.com:8001)
[client](http://a34e2b87c1ce74d11a2f8c816dd38ccc-370286170.ap-south-1.elb.amazonaws.com)
