Based on [express-4.x-github-example](https://github.com/stefandesu/express-4.x-github-example) (which in turn is based on [express-4.x-facebook-example](https://github.com/passport/express-4.x-facebook-example)), using [passport-orcid](https://github.com/hubgit/passport-orcid).

This example demonstrates how to use [Express](http://expressjs.com/) 4.x and
[Passport](http://passportjs.org/) to authenticate users using ORCID.  Use
this example as a starting point for your own web applications.

For the official example from the passport-orcid repository, see [here](https://gitlab.coko.foundation/pubsweet/passport-orcid/blob/master/example/index.js).

## Instructions

To install this example on your computer, clone the repository and install
dependencies.

```bash
$ git clone https://github.com/stefandesu/express-4.x-orcid-example.git
$ cd express-4.x-orcid-example
$ npm install
```

The example uses environment variables to configure the consumer key and
consumer secret needed to access ORCID's API. You can go [here](https://support.orcid.org/knowledgebase/articles/343182) to create a new OAuth application for ORCID.  Start the server with those
variables set to the appropriate credentials.

```bash
$ CLIENT_ID=__ORCID_CLIENT_ID__ CLIENT_SECRET=__ORCID_CLIENT_SECRET__ node server.js
```

Alternatively, you can provide a `.env` file in the following form:
```bash
CLIENT_ID=__ORCID_CLIENT_ID__
CLIENT_SECRET=__ORCID_CLIENT_SECRET__
PORT=__EXPRESS_PORT__
```

Open a web browser and navigate to [http://localhost:3000/](http://localhost:3000/)
(adjust port if necessary) to see the example in action.
