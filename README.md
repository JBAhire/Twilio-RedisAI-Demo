# Twilio-RedisAI-Demo
In this demo I will be demoying an image labelling using redisAI and we will display our result using Twilio WhatsApp API. This interactive demo can give you good insights of twilio API's as well as AI capabilities of Redis.

# Prerequisites
* A Twilio account - sign up for a free one here
* A Twilio phone number with SMS capabilities - configure one here
* Set up your Python and Flask developer environment - Make sure you have Python 3 downloaded as well as ngrok.
* Redis with RedisAI module
* Models are already here in models folder.

# Installation for Redis
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
# Installation for RedisAI
You can find instructions to launch docker instance or build RedisAI from source here: https://github.com/RedisAI/RedisAI

# Setup and Demo:
* Start Redis-Server with redisAI module or launch redisAI docker instance. [ you can find instructions at https://github.com/RedisAI/RedisAI ]

* Run Demo.py file

* Your Flask app will need to be visible from the web so Twilio can send requests to it. Ngrok lets us do this. With it installed, run the following command in your terminal in the directory your code is in. Run ```ngrok http 5000``` in a new terminal tab.

* Grab that ngrok URL to configure twilio whatsapp sandbox.

* Follow the instructions on twilio whatsapp sandbox website to join the sandbox.

* send any photo on the chat and see the result!

# If you want to know more about this and how this works please check out my blog post here: 








