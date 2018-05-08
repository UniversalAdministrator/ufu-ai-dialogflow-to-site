# A Simple UfU Webhook for DialogFlow with Node.js.

This is a pretty simple node.js app that serves as a fulfilment service for DialogFlow agents. 

# Up and running in 2 steps

1. Deploy this webhook to heroku

    [![Deploy to Heroku](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

2. Activate the Webhook in DialogFlow with the url provided by heroku 

 [webhook documentation](https://docs.api.ai/docs/webhook)


You can check out [Rich Messages](https://docs.api.ai/docs/rich-messages) and [Response design for Actions on Google](https://docs.api.ai/docs/response-design-for-actions-on-google) for other types of responses.

# Tools for Development

We of course need to develop and test the webhook before being deployed to the host. Below are the utilities I used. 

* [Postman](https://chrome.google.com/webstore/detail/postman/fhbjgbiflinjbdggehcddcbncdddomop) - Use it to send some test payloads to the webhook. So I don't need to "talk" using api.ai during initial tests.

* [ngrok](https://ngrok.com/) - Creates a public https tunnel mapped to a port on my machine. It gives me a url that I can use as a webhook for my agent. Use this to actually integrate your agent to the webhook.

* [heroku-cli](https://devcenter.heroku.com/articles/heroku-cli) - Well, only if you'll be deploying to heroku.

