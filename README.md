[![Voicybot](/img/logo.png?raw=true)](http://voicybot.com/)

# [@voicybot](https://t.me/voicybot) main repository
This repository contains the code for one of the most popular bots I've ever built for Telegram — [@voicybot](https://t.me/voicybot). Please, feel free to fork, add features and create pull requests so that everybody (over 500 000 chats) can experience the features you've built.

# List of repositories
* [Voicy](https://github.com/backmeupplz/voicy) — the main [@voicybot](https://t.me/voicybot) code
* [Voicy localizations](https://github.com/backmeupplz/voicy-localizations) — the list of localized strings for [@voicybot](https://t.me/voicybot)
* [Voicy payments](https://github.com/backmeupplz/voicy-payments) — payments service that used stripe to process payments for the Google Speech seconds of recognition; currently retired as a stats server for [voicybot.com](http://voicybot.com)
* [Voicy landing](https://github.com/backmeupplz/voicy-landing) — [voicybot.com](http://voicybot.com) landing page


# Installation and local launch
1. Clone this repo: `git clone https://github.com/backmeupplz/voicy`
2. Launch the [mongo database](https://www.mongodb.com/) locally
3. Create `.env` file with the environment variables listed below
4. Run `yarn install` in the root folder
5. Run `yarn start`

# Environment variables in `.env` file
* `MONGO_URL` — Url for the mongo database used
* `TOKEN` — Telegram bot token
* `SALT` — Random salt to generate various encrypted stuff
* `ADMIN_ID` — Chat id of the person who shall receive valuable logs
* `YANDEX_KEY` — Key for Yandex SpeechKit voice recognition service 
* `USERNAME` — Username of the bot in the format `bot_bot_bot`
* `WIT_LANGUAGES` — A map of language names to Wit.ai tokens

Extra info is available in `.env.sample` file.

# Continuous integration
Any commit pushed to master gets deployed to [@voicybot](https://t.me/voicybot) via [CI Ninja](https://github.com/backmeupplz/ci-ninja).

# License
MIT — use for any purpose. Would be great if you could leave a note about the original developers. Thanks!

# As seen on
[![Habrahabr](/img/habr.png?raw=true)](https://habrahabr.ru/post/316824/)
[![Spark](/img/spark.png?raw=true)](https://spark.ru/startup/voicy/blog/19008/kak-zapustit-proekt-v-odinochku/)
[![Reddit](/img/reddit.png?raw=true)](https://redd.it/5iduzy)
[![Bot Store](/img/bs.png?raw=true)](https://storebot.me/bot/voicybot)
[![Product Hunt](/img/ph.png?raw=true)](https://www.producthunt.com/posts/voicy)

# TODO
* Google speech credentials integration
* Turn off censorship
* Localizations
* Make channels work again
* Check different file types again