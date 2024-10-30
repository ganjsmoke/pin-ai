# Multi-Account Auto Pin AI Bot

This bot is designed to interact with multiple accounts using the Pin AI API. The bot is equipped with an invite checker that uses the specified invite code. 

## 🔗 Use My Invite Link

If you want to use this bot, you can start by using my invite link: [Use this Invite Link](https://t.me/hi_PIN_bot/app?startapp=p56x6s3).

## Features

- **Multi-Account Management:** Handles multiple accounts stored in `accounts.json`.
- **Token Refresh:** Automatically refreshes access tokens when expired.
- **Task Automation:** Completes tasks, claims coins, and upgrades the model for each account.

## Installation

Follow the instructions below to clone and install the bot:

### 1. Clone the Repository

```
git clone https://github.com/ganjsmoke/pin-ai.git
```
```
cd pin-ai
```


### 2. Install Dependencies

The required dependencies are listed in the `package.json` file. To install them, run:

```
npm install
```

This command will install all the necessary modules automatically.

## Configuration

1. **Create `accounts.json` file**: 
   - The bot requires an `accounts.json` file to store account details.
   - Create a file named `accounts.json` in the root directory of the project.
   - Structure of `accounts.json`:
     ```json
     {
         "accounts": [
             {
                 "init_data": "<init_data_value>",
                 "access_token": "<access_token_value>",
                 "refresh_token": "<refresh_token_value>"
             }
         ]
     }
     ```
     you can leave blank for access_token and refresh token and it will populate


## Running the Bot

To start the bot, simply run:

```
node index.js
```

The bot will run continuously in an infinite loop, processing accounts and refreshing every 1 hours.
