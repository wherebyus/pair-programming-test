Hello!
This repo contains a handful of different pair programming exercises
we use for interviews. Your interview will probably only involve one,
and if you're reading this you should know which one.

The goal of these exercises is to gauge where you're at technically,
and see how you perform in an environment similar to what you'll experience at Cozy.
We want to make sure you can be successful and happy in a highly collaborative environment;
we don't particularly care if you know obscure features of RSpec
or know everything about promises.

The instructions for getting each exercise up and running are in this README.
When possible, please make sure you go through those steps beforehand,
and tell your interviewer if you run into any problems.

The actual steps/requirements of the exercise will be discussed during the interview.

Ruby TDD
===

For this exercise, we'll do some simple TDD exercises.
The repo contains some placeholder code to demonstrate specs working.

Make sure you have Ruby 2.2+ and rspec 3.0+ installed (we're using Ruby 2.2 and RSpec 3.2).
You can use rbenv/RVM and bundler for this, or install into system Ruby, whatever you want.
There are a few helper files already in the repo to make using a version manager and bundler easier for you.
Ideally it's just a `bundle install` in the `ruby-tdd` directory.

Logic goes in `app.rb` and specs go in `specs.rb`.

Once you're all set up, run the specs to make sure things are working:

```
$ cd ruby-tdd/
$ rspec specs.rb 

the programming test
  works on my machine!

Finished in 0.00084 seconds (files took 0.11766 seconds to load)
1 example, 0 failures
```

The existing code in `app.rb` and `specs.rb` can be cleared out.


Weather Service
===

This exercise involves writing a client to render weather information from
a server. We will refactor and improve the client.

First we need to get the server running.
Ensure you have a relatively current version of Node and NPM installed.
Your interviewer will send you an API key for OpenWeatherMap.org.
We'll need to install dependencies, export the key, and start the server:

```
$ cd weather-service-node
$ npm install
$ export OPENWEATHER_API_KEY=YOUR_KEY
$ node index.js
Serving on http://localhost:3000
```

In another shell, ensure the server is working:

```
$ curl http://localhost:3000/weather
{"city":"Portland","country":"US","temp":26.480000000000018,"tempMin":25,"tempMax":28.33000000000004,"weather":"Clouds","windSpeed":3.1,"windDirection":20}
```

The client is a static client hosted in another directory.
All you need to do is run an HTTP server:

```
$ cd weather-client
$ python -m SimpleHTTPServer 1025
Serving HTTP on 0.0.0.0 port 1025 ...
```

Finally, open a browser to `http://localhost:1025`.
Press the button and ensure everything is working.
