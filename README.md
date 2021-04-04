# Netcup Easteregg Crawler
To use the crawler just run `./netcup_crawler.py`.

It will first crawl for different pages and saves them in the file `urls.txt`.
After that it will use the api to check if there are any easter eggs.

To specify what offer you are looking for, set the `search_for_offer` variable, e.g.:
```python
search_for_offer = "VPS Ostern L" # specify a offer to search for
```

The offers are limited, if your desired one is found, try to buy it as quick as possible.
If its out of stock, just let the crawler run during the day. They will add new ones from time to time.

## Use a telegram bot
If you want you can specify the data of your telegram bot to receive a message when your desired offer is found:
```python
telegram_use        = True
telegram_bot_token  = "123123:AAAABBBCCC..."
telegram_chat_id    = "123456"
telegram_amout_msgs = 10 # amount of message you will receive if your offer is found
```

## Skip the crawling phase
To skip the crawling phase use `./netcup_crawler.py --skip-crawling`. But ensure the url.txt file with the urls to check are available then!
