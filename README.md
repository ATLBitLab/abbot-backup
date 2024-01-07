# Abbot
A helpful bitcoiner bot at [ATL BitLab](https://atlbitlab.com/abbot). Est. block 797812.

## Summary
Abbot stands for **A**tl **B**itlab **Bot**. 

Basic tasks that Abbot can automate include:
1. Content gathering and organization
2. Content creation
3. Answering questions about ... anything!
4. Nostr, Twitter posting
5. Automating tasks for meetup community organizers

## Requirements
- Python >= 3.11.6 
- Telegram bot API key
  - DM the [Bot Father](https://www.telegram.me/BotFather)
  - Recommend creating 2 bots: @your_telegram_bot and @test_your_telegram_bot
  - See step 7. for how this comes in handy
- OpenAI API key
  - Create an account at [https://platform.openai.com](https://platform.openai.com) 
  - Go create an API key [https://platform.openai.com/account/api-keys](https://platform.openai.com/account/api-keys)
- Must have a lightning payment method
  - Abbot is shipped with a Strike Merchant integration and requires a Strike API key out-of-the-box
  - We are working on offering multiple payment ingtegrations
  - Feel free to fork and contribute to [#2](https://github.com/ATLBitLab/abbot/issues/2)

## Install & Run
1. Clone repo && go to dir
```
git clone https://github.com/ATLBitLab/abbot.git && cd abbot
```

2. Copy sample env file into `lib/`
```
cp .env.sample src/.env
```

3. Enter your keys into the appropriate positions

4. Create virtual env
```
python -m venv .venv
```

5. Activate virtual env
```
source .venv/bin/activate
```

6. Install requirements.txt
```
pip3 install -r requirements.txt
```

7. If you created a test bot per the #requirements section, you can run the test bot
```
cd src
python main.py --dev
```

8. Go to your telegram and DM your bot! That's it!

Found bugs? Need help? Submit a [Bug Report Issue](https://github.com/ATLBitLab/abbot/issues/new?assignees=&labels=&projects=&template=bug_report.md&title=)
Feel free to contact me: https://nonni.io
