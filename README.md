Hello!
This repo contains a handful of different pair programming exercises
we use for interviews. Your interview will probably only involve one,
and if you're reading this you should know which one.

The goal of these exercises is to gauge where you're at technically,
and see how you perform in an environment similar to what you'll experience at WBU.
We want to make sure you can be successful and happy in a highly collaborative environment;
we don't particularly care if you know obscure features of RSpec.

Ideally we are working on your machine,
either remotely or at the WhereBy.Us office.
Programming is much easier when you're using familiar equipment and tools!
Instructions for remote pairing will be sent out ahead of the interview.

The instructions for getting each exercise up and running are in this README.
When possible, please make sure you go through those steps beforehand,
and tell your interviewer if you run into any problems.

The actual steps/requirements of the exercise will be discussed during the interview.


Ruby TDD
===

For this exercise, we'll do some simple Test Driven Development
using Ruby.
The specific exercise will depend on your experience and the role you're applying for.

There are no libraries other than the Ruby standard library and RSpec required.
The repo contains some placeholder code to demonstrate specs working.

Instructions
=====

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

