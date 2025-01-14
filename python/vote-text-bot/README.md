# Google Chat Vote bot sample (text-only)

This code sample creates a Google Chat simple text-only Vote bot that
allows a user to vote (+1 or -1) on a message. This implementation is
written in Python and hosted on Google App Engine.

![Vote bot (text-only)](https://user-images.githubusercontent.com/744973/43745610-9fdfc1c4-9994-11e8-9f47-b16fe3438458.png)

## Run the sample

To run this sample, you must follow these directions to create an App Engine
project, create the bot and publish it for yourself in your G
Suite domain, pointing Google Chat to your App Engine-based bot.
Once it's published, you can find the bot and add it to a chat room or
direct message.

1. [Install the Google Cloud SDK](https://cloud.google.com/sdk/downloads)
  if you haven't already and ensure the `gcloud` command works.
1. [Create a new Google Cloud Platform project](https://console.cloud.google.com)
  or select an existing project.
1. Create an App Engine app (or use an existing one) and note the
  `_APP-ID_.appspot.com` domain you get by default (customize as desired).
1. Create a new folder and drop the files for this bot in it. From there,
  [deploy your App Engine app](https://cloud.google.com/appengine/docs/standard/python/tools/uploadinganapp#deploying_an_app).
1. Now follow the instructions to
  [publish your bot to Google Chat](https://developers.google.com/chat/how-tos/apps-publish)
1. On the [Google Chat Configuration
  tab](https://console.developers.google.com/apis/api/chat.googleapis.com/hangouts-chat),
  customize your bot by setting the following values:
  - **Project name**: "Vote bot"
  - **Bot name**: "Vote bot"
  - **Avatar URL**: `https://www.gstatic.com/images/icons/material/system/2x/how_to_vote_black_48dp.png`
  - **Description**: "Vote bot"
  - **Functionality**: enable for (at least) chat rooms
  - **Connection settings**: select _Apps Script_ and add _Deployment ID_ (per general directions above)
  - **Permissions**: select _Specific people and groups in your domain_, and enter your G Suite email address
1. Click **Save changes** to publish your bot
1. Add the Vote bot to a chat room and see a new message from the bot with
  the vote card ready to accept its first vote!

## Reference

- [Creating Google Chat interactive cards](https://developers.google.com/chat/api/guides/message-formats/cards) featuring the same vote bot that supports images and hosted on [Google Cloud Functions](https://cloud.google.com/functions)
- [Google Chat bot concept page](https://developers.google.com/chat/how-tos/apps-develop)
- [Creating new bots in Google Chat](https://developers.google.com/chat/how-tos/apps-develop)
- [Google Chat developer documentation](https://developers.google.com/chat)
- [Google App Engine product documentation](https://cloud.google.com/products/appengine)
- [Python App Engine (standard) documentation](https://cloud.google.com/appengine/docs/standard/python/)
