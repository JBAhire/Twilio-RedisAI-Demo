# Twilio-RedisAI-Demo
This is the code for the demo I shown in Redis Day Banaglore. In this demo I will be demoying an image labelling using redisAI and we will display our result using Twilio WhatsApp API. This interactive demo can give you good insights of twilio API's as well as AI capabilities of Redis.

## Prerequisites
* A Twilio account - [sign up for a free one here](https://www.twilio.com/try-twilio)
* A Twilio whatsapp sandbox - [configure one here](https://www.twilio.com/console/sms/whatsapp/sandbox)
* [Set up your Python and Flask developer environment](https://www.twilio.com/docs/usage/tutorials/how-to-set-up-your-python-and-flask-development-environment) - Make sure you have Python 3 downloaded as well as [ngrok](https://ngrok.com/).
* [Redis](https://github.com/antirez/redis) with [RedisAI](https://github.com/RedisAI/RedisAI) module
* Models are already here in models folder.

## Installation for Redis
Download, extract and compile Redis with:
```
$ wget http://download.redis.io/releases/redis-5.0.7.tar.gz
$ tar xzf redis-5.0.7.tar.gz
$ cd redis-5.0.7
$ make
```
The binaries that are now compiled are available in the ```src``` directory. Run Redis with: 
```
$ src/redis-server
```
You can interact with Redis using the built-in client:
```
$ src/redis-cli
redis> set foo bar
OK
redis> get foo
"bar"
```
## Installation for RedisAI
You can find instructions to launch docker instance or build RedisAI from source here: https://github.com/RedisAI/RedisAI

## Setup and Demo:
* Start Redis-Server with redisAI module or launch redisAI docker instance. [ you can find instructions at https://github.com/RedisAI/RedisAI ]

* Run Demo.py file

* Your Flask app will need to be visible from the web so Twilio can send requests to it. Ngrok lets us do this. With it installed, run the following command in your terminal in the directory your code is in. Run ```ngrok http 5000``` in a new terminal tab.

* Grab that ngrok URL to configure twilio whatsapp sandbox.

* Follow the instructions on twilio whatsapp sandbox website to join the sandbox.

* send any photo on the chat and see the result!

## If you want to know more about this and how this works please check out my blog post here: 








