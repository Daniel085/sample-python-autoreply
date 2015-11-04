sample-python-autoreply
===

Basic auto-reply application using Python, Tweepy and NLTK.

To run this sample code, you'll need to install the following python libraries:

- Tweepy: [https://github.com/tweepy/tweepy](https://github.com/tweepy/tweepy)
- NLTK: [http://www.nltk.org/](http://www.nltk.org)


Getting Started
---
Create a [Twitter App](https://apps.twitter.com/).

Specify your Twitter App keys and tokens in a new config file named .twitter. There is a sample config file named .twitter.sample:

```
[apikey]
key = your_api_key
secret = your_api_secret

[token]
token = your_access_token
secret = your_access_secret

[app]
rule = @AccountOwnerOfApp
account_screen_name = AccountOwnerOfApp
account_user_id = UserIdOfAccountOwner

```

Install dependencies:

```
pip install tweepy nltk
```

Run the python script in the project directory:

```
python AutoResponse.py
```

Notes
-----
Currently this code is not fully Python 3.x-compatible and may need some work, but should work fine on Python 2.7

This is a very barebones code example to get you started. There are additional considerations you should account for in your application. Please familiarize yourself with the following to help you create the best experience for yourself and your users.

[The Twitter Rules](https://support.twitter.com/articles/18311-the-twitter-rules)<br/>
[Automation Rules & Best Practices](https://support.twitter.com/articles/76915)<br/>
[API Rate Limiting](https://dev.twitter.com/rest/public/rate-limits)
