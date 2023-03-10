# WhatsApp API Webhook

Webhooks allows you to receive real-time HTTP notifications of changes to specific objects. For example, we could send you a notification when a user sends you a message or when a message template's status has changed. This prevents you from having to query our APIs for changes to objects that may or may not have happened, and helps you avoid reaching your rate limit.

This document provides an overview of Webhooks and they apply to the WhatsApp Business Management API, WhatsApp Business Platform Cloud API, and WhatsApp Business Platform On-Premises API.

---

## Requirements

For development, you will only need Node.js and a node global package, Yarn, installed in your environement.

### Node

- #### Node installation on Windows

  Just go on [official Node.js website](https://nodejs.org/) and download the installer.
  Also, be sure to have `git` available in your PATH, `npm` might need it (You can find git [here](https://git-scm.com/)).

- #### Node installation on Ubuntu

  You can install nodejs and npm easily with apt install, just run the following commands.

      $ sudo apt install nodejs
      $ sudo apt install npm

- #### Other Operating Systems
  You can find more information about the installation on the [official Node.js website](https://nodejs.org/) and the [official NPM website](https://npmjs.org/).

If the installation was successful, you should be able to run the following command.

    $ node --version
    v8.11.3

    $ npm --version
    6.1.0

If you need to update `npm`, you can make it using `npm`! Cool right? After running the following command, just open again the command line and be happy.

    $ npm install npm -g

## Install

    $ git clone https://github.com/shahzamaahmad/whatsapp-api
    $ cd whatsapp-api
    $ npm install

## Configure app

Create `.env` then edit it with your settings. You will need:

- VERIFY_TOKEN=TOKEN_NAME,
- WHATSAPP_TOKEN=your_whatsapp_token,
- PORT=1337,

## Running the project

    $ DEBUG=whatsapp-api:* npm start

## Simple build for production

    $ npm start
