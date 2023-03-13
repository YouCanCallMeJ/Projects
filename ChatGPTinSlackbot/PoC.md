# ChatGPTinSlackbot PoC
## Architecture
* Slack
    * Provides a webhook to post a message as a slackbot
    * Provide an endpoint 
* Glitch
    * Run a NodeJS server.js file to listen to the slackbot event
    * Send HTTP request to the ChatGPT API endpoint and get the result
    * Post a slack message with the BOT_TOKEN into the slack 

## What
* I want to have:
    * A slackbot that forwards my inputs to the ChatGPT and returns output from the ChatGPT

## How
1. Create a slackbot and Configuration
2. Create a server/app to listen to the slackbot event
3. Update the server to send HTTP request to the ChatGPT and get the result from the ChatGPT
4. Post a message from the server to the Slack using BOT_TOKEN

## Reference
* https://api.slack.com/events/message
* https://dreisbach.us/articles/build-slackbot-glitch/
* https://blog.logrocket.com/build-a-slackbot-in-node-js-with-slacks-bolt-api/
* https://dev.to/codesphere/create-a-slack-bot-with-nodejs-215e
* https://platform.openai.com/docs/api-reference/chat/create
* https://github.com/pedrorito/ChatGPTSlackBot