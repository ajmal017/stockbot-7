# Welcome to your CDK TypeScript project!

This is a blank project for TypeScript development with CDK.

The `cdk.json` file tells the CDK Toolkit how to execute your app.

## Useful commands

 * `npm run build`   compile typescript to js
 * `npm run watch`   watch for changes and compile
 * `npm run test`    perform the jest unit tests
 * `cdk bootstrap`   create assets (Docker required)
 * `cdk deploy`      deploy this stack to your default AWS account/region
 * `cdk diff`        compare deployed stack with current state
 * `cdk synth`       emits the synthesized CloudFormation template

## Prerequisites
 * AWS CLI
 * AWS CDK
 * An AWS CLI profile with permissions to deploy architecture
 * AWS SAM CLI – beta

## Telegram bot

Simply open these commands in your browser

 * To set a webhook
   ``
   https://api.telegram.org/bot{bot_token}/setWebhook?url={webhook_url}
   ``

 * To delete a webhook
   ``
   https://api.telegram.org/bot{bot_token}/deleteWebhook
   ``

 * To get information about your webhook
   ``
   https://api.telegram.org/bot{bot_token}/getWebhookInfo
   ``

see also the section [getting started](https://core.telegram.org/#getting-started) of Telegram API

## Local test

* To invoke lambda locally 
  ``
  sam-beta-cdk local invoke LambdaHandlers/TelegramHandler -e events/telegram.json -n locals.json
  ``
* 

see also the [reference](https://aws.amazon.com/tw/blogs/compute/better-together-aws-sam-and-aws-cdk/) about aws sam