Mozilla Watcher
=====

This script watches the Mozilla GitHub organizations and saves the newly discovered repositories. It
also saves the newly edited wiki pages.

Setting up the server
-----

First install [Docker](https://docs.docker.com/install/) and [docker-compose](https://docs.docker.com/compose/install/).

Then you can start the server with the following command. Make sure to replace the placeholders with your data.

```
$ git clone <URL>
$ npm install
$ GITHUB_TOKEN=<yourGitHubToken> docker-compose up
```

Now you can access the website for it at ```localhost:3000```.

Running the fetch script
------

The fetch script can be run to make sure the website has the latest information. It automatically refreshes itself when running with `npm start`, so this is only needed for updates additionally to that.

```
$ npm run fetch
```
