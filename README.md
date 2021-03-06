
# Finally Comments

The aim of this project is to promote the Steem ecosystem by breaking the comments system out of the walls of Steem based apps.

## Finally comments - V0.7.0
An embededable version of steem (steemit/utopian) comments with comment and vote functionality

### How It Works
[Please visit the site for more detaails](http://finallycomments.com)

Finally is an evolution of Steemcomments.js and at its core uses the Steem blockchain to provide posting and curation rewards to its users. Similar to other popular plug and play comment systems Finally requires only a single html tag while our javascript library & backend system take care of the rest.

Login to the dashboard at [http://finallycomments.com](http://finallycomments.com/auth/dashboard). to generate code for any Steemit(or any other STEEM based platform) post with one click.
```
  <section class="finally-comments" data-id="https://utopian.io/utopian-io/@sambillingham/tutorial-beginner-friendly-build-your-first-steem-bot-in-javascript-30minutes"></section>
  <script src="https://finallycomments.com/js/finally.min.js"></script>

```
![](http://i66.tinypic.com/5ozia8.jpg)

Finally uses Steemconnect authentication to allow users to post comments and upvotes directly from anywhere Finally is embeded. Once authenticated with Finally users will not have to log in again when visiting other sites that also use Finally.

*Currently Finally only supports content already posted to the Steem network. Sites including Steemit, Busy or Utopian. Support for more sites (dmania/dsound/dtube/dlive) will be added shortly and in the comming weeks support for content outside of the Steem blockchain will be enabled.*

### Development Setup
You'll need to create an account on steemconnect.com to work on this project (current cost 3 STEEM). Use the details within the finallycomments app. Make sure the redirect url matches.

start by passing enviroment varibles to the node process for example
```
git clone
cd app/
npm install
NODE_CLIENT_ID="newproject.app" NODE_REDIRECT_URI="localhost:3000/auth/" NODE_SESSION_SECRET="supersecret27" node ./bin/www
```

### Feature Roadmap
- stats for threads/account
- auto hide posts from rep less than X
- edit/delete/flag comments
- moderate comments (completely remove with flag from author)
- wordpress plugin
- non logged in user comments (not expected for some time)
