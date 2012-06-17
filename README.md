**IMPORTANT** Chronologic has been end-of-life'd. It's no longer in production, but it's still an OK piece of software. [Would you like to know more?](http://weblog.therealadam.com/2012/06/17/chronologic-a-piece-of-software-history/)

# Chronologic: You put your feeds in it

Chronologic is a service for storing and generatin activity feeds, new
feeds, timelines, and other forms of aggregated, reverse-sorted data.
Chronologic includes a small model layer that applications can use to
map their domain to Chronologic types. This model layer talks to a
Chronologic REST service. Said service uses an underlying database for
storage. Currently storage is Cassandra-only, but that's a temporary
condtion, you dig?

## Overview

Chronologic exposes four kinds of data:

* **Events** are the items that appear in your feeds. These are your
  statuses, checkins, commits, changes, etc. Feeds are often a social
  thing, therefore they reference objects...
* **Objects** are the things that events happen to. These are your
  users, spots, projects, documents, etc.
* **Timelines** are the endpoints where activity feeds appear. They
  contain any number of events. Every event is written to one or more
  target timelines. Timelines fan events out based on subscriptions...
* **Subscriptions** connect timelines to other timelines. To make events
  posted to your user timeline appear in the site-wide timeline, you
  would subscribe the site-wide timeline to your use timeline.

## Hello, Chronologic

An example goes here.

## Running Chronologic

Instructions on running Chronologic and idea about deploying it go here.

## Contributing

The way you contribute to the development of Chronologic goes here.

## License

Copyright 2010-2011 Gowalla Incorporated. Chronologic is MIT licensed.

