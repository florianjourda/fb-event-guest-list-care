# Facebook Event Guest List Care

This is a sample client for [Facebook's Graph API Webhooks](https://developers.facebook.com/docs/graph-api/webhooks/) and [Instagram's Subscriptions API](https://www.instagram.com/developer/subscriptions/), powered by [Node.js on Heroku](https://devcenter.heroku.com/articles/getting-started-with-nodejs).

## Setup

### Heroku
1. Deploy with this button: [![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/florianjourda/fb-event-guest-list-care)
1. Test your deployment with `curl https://<your-subdomain>.herokuapp.com` - you should see "It works!".
1. For handling POST request validation (optional, but suggested), set the `APP_SECRET` [config var](https://devcenter.heroku.com/articles/config-vars) using your app secret value from your [Facebook app's settings](https://developers.facebook.com/apps).

### Facebook
1. Create a new [Facebook application](https://developers.facebook.com/apps).
1. Set up your Facebook application's [Graph API Webhooks subscription](https://developers.facebook.com/docs/graph-api/webhooks/#setup) using `https://<your-subdomain>.herokuapp.com/facebook` as the callback URL and `token` as the verify_token.

### Instagram
1. Register an [Instagram API client](https://instagram.com/developer/clients/manage/).
1. Set up your client's [subscription](https://www.instagram.com/developer/subscriptions/) using your `https://<your-subdomain>.herokuapp.com/instagram` as the callback URL and `token` as the verify_token.
