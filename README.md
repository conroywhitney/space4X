# Space 4X
A [4X](http://en.wikipedia.org/wiki/4X) [tick-based](http://en.wikipedia.org/wiki/Turns,_rounds_and_time-keeping_systems_in_games#Ticks_and_rounds) [MMORPG](http://en.wikipedia.org/wiki/Massively_multiplayer_online_role-playing_game) designed as an exercise in [parallel](http://en.wikipedia.org/wiki/Parallel_computing), [distributed](http://en.wikipedia.org/wiki/Distributed_computing), [agent-based](http://en.wikipedia.org/wiki/Agent-based_model) computing.

This repository is for the game mechanics, tests, and API server infrastructure that may later be used by web, mobile, and tablet clients.

## 4X Tick-Based MMORPG
[MMO](http://en.wikipedia.org/wiki/Massively_multiplayer_online_role-playing_game) games require scale and distribution to function smoothely for all players. [Tick-based]((http://en.wikipedia.org/wiki/Turns,_rounds_and_time-keeping_systems_in_games#Ticks_and_rounds) games require that iteractions are processed simultaneously in one huge burst, instead of spread out over time. [4X](http://en.wikipedia.org/wiki/4X) games set a framework for thinking about objects as agents. Combined, these provide a suitable context in which to develop a [parallel](http://en.wikipedia.org/wiki/Parallel_computing), [distributed](http://en.wikipedia.org/wiki/Distributed_computing), [agent-based](http://en.wikipedia.org/wiki/Agent-based_model) program.

Personal inspiration includes [Planetarion](http://en.wikipedia.org/wiki/Planetarion) and [Age of Empires II](http://en.wikipedia.org/wiki/Age_of_Empires_II:_The_Age_of_Kings).

## Parallel
Models and functions are designed to be manipulated in parallel through the use of:
* [Ruby Closures](http://innig.net/software/ruby/closures-in-ruby)
* [Scala](http://en.wikipedia.org/wiki/Scala_(programming_language)
* [Resqueue](https://github.com/defunkt/resque)
* [Mongo Atomic Transactions](http://www.mongodb.org/display/DOCS/Atomic+Operations)

## Distributed
Designed to scale from 1 to N computers in a cluster on EC2 or any other grid/cloud platform through the use of:
* [Message Queues](http://en.wikipedia.org/wiki/Message_queue)
* [Horizontal Scaling](http://en.wikipedia.org/wiki/Scalability#Scale_horizontally_.28scale_out.29)
* [Sharding](http://en.wikipedia.org/wiki/Shard_(database_architecture))

## Agent-Based
Instead of having a "god" commanding the program, each patch, body, object, etc. is autonomous and reacts to the outside world based on stimuli. This goal is inspired by [Turtles, Termites, and Traffic Jams](http://www.amazon.com/Turtles-Termites-Traffic-Jams-Explorations/dp/0262680939) which uses [StarLogo](http://en.wikipedia.org/wiki/StarLogo) to show how complex macro-patterns can arise from many simple micro-decisions.
