Install ask-cli and initialize it
```
npm install -g ask-cli
ask-cli init
```
Edit .ask/congig.template with your skill id and Lambda ARN

To generate the catalog files:

Install and configure awscli
Create user, roles and DynamoDB table, Drobpbox token as described here: medium-link-here

Edit .env.template with your Dropbox token and rename to .env
```
$ cd dropbox-catalog
$ npm install
$ node index.js upload -d ./mp3/
$ node index.js catalog
```

Upload catalog files as described in the medium article

Deploy the skill and lambda
```
$ ask deploy
```