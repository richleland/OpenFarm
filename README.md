OpenFarm
========

OpenFarm ([OpenFarm.cc](http://openfarm.cc)) is a free and open database for farming and gardening knowledge. One might think of it as the Wikipedia or Freebase for growing plants. The data is crowdsourced and includes all of the necessary paramaters for a machine or human to successfully grow a plant, ie: seed spacing and depth, water regimen, recommended soil composition and companion plants, sun/shade requirements, etc.

This project is closely related to the FarmBot project but also distinctly separate. OpenFarm is a standalone database that will simply provide data to other applications. For FarmBot, OpenFarm will supply the default settings to grow a plant when a user selects it in the graphical FarmBot frontend.

OpenFarm will also have a web frontend of its own to allow anyone to access the data and make contributions.

Examples of other applications using OpenFarm: a mobile application for home gardeners, Google providing "One Box" answers to search queries such as "How do I grow tomatoes", Wolfram Alpha displaying the data for "growng tomatoes" which is also showed to users asking Siri on iDevices, etc.

### Issue Tracker

[![Stories in Ready](https://badge.waffle.io/FarmBot/OpenFarm.png?label=ready)](http://waffle.io/FarmBot/OpenFarm)

### Getting Started (Setup)

You will need [Ruby](http://www.ruby-lang.org/en/), [Rails](http://rubyonrails.org/) and [Mongodb](http://docs.mongodb.org/manual/installation/) installed. To get started with a local copy of the project, run:

```bash
$ git clone https://github.com/FarmBot/OpenFarm.git
$ cd OpenFarm
$ bundle install
$ rake db:migrate
$ rails s
```

If all went well, you will have a seeded database and can use the account `admin@admin.com` with password `admin123`.

#### OAuth

OpenFarm supports OAuth through Facebook and Twitter, however you have to enable it yourself.

For Twitter, you need to set the `TWITTER_CONSUMER_KEY` and `TWITTER_CONSUMER_SECRET` environment variables before starting the server:

```bash
export TWITTER_CONSUMER_KEY=my-consumer-key
export TWITTER_CONSUMER_SECRET=my-consumer-secret
rails s
```

For Facebook it is the same way, except the fields are `FACEBOOK_APP_ID` and `FACEBOOK_APP_SECRET`.

### How to Contribute

 1. Fork this repo.
 2. Fix stuff, add features.
 3. Send pull request to master.

Not sure where to help? Take a look [over here](http://waffle.io/FarmBot/OpenFarm).

### FAQ

Have a look at the [FAQ](https://github.com/FarmBot/OpenFarm/wiki/FAQ) for some frequently asked questions about contributing (Angular, Issue Trackers, IRC Channels). 

### User Flow

![User Flow Diagram] (http://i.imgur.com/YowIq1N.jpg)

![Information Architecture Diagram] (http://i.imgur.com/qZzF4OZ.jpg)

### Mockups

To view the most recent mockups, click [here] (https://drive.google.com/open?id=0B-wExYzQcnp3cVZvZ3JXb3FDZTg&authuser=0)

### Contributors

[https://github.com/FarmBot/OpenFarm/graphs/contributors](https://github.com/FarmBot/OpenFarm/graphs/contributors)

### License

The MIT License (MIT)

Copyright (c) 2014 Farmbot Project, et. al. [(http://go.farmbot.it/)](http://go.farmbot.it/)

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

### Data License

The data within the OpenFarm.cc database is licensed under the [Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by/4.0/)

[![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/FarmBot/openfarm/trend.png)](https://bitdeli.com/free "Bitdeli Badge")

