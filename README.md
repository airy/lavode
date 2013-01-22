# Lavode

Lavode is customized [hubot][hubot] version of GitHub's hubot with mongo-brain.
She lives in [Heroku][heroku] and talk in [Talker][talker].

[heroku]: http://www.heroku.com
[talker]: http://talkerapp.com
[hubot]: http://hubot.github.com

## Playing with lavode

### Mongo brain on Heroku

If you are going to use the `mongo-brain.coffee` script from `hubot-scripts`
you will need to add the Mongolab addon on Heroku which requires a verified
account or you can create an account at [Mongolab][mongolab] and manually
set the `MONGOLAB_URL` variable.

    $ heroku config:add MONGOLAB_URL="..."

[mongolab]: https://mongolab.com/

### Talker

You need to set HUBOT_TALKER_TOKEN and HUBOT_TALKER_ROOMS variables.

heroku

    $ heroku config:add HUBOT_TALKER_TOKEN="..."
    $ heroku config:add HUBOT_TALKER_ROOMS="111,222"

local

    $ export HUBOT_TALKER_TOKEN="..."
    $ export HUBOT_TALKER_ROOMS="111,222

### Test Lavode Locally

You can test your lavode by running the following.

    $ bin/hubot 
