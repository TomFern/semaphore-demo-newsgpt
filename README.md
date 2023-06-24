# semaphore-demo-newsgpt

This is **NewsGPT**, an OpenAI GPT-3 chatbot that can look up news for you.

The goal of project is to show how to implement OpenAI's [function calling](https://platform.openai.com/docs/guides/gpt/function-calling) feature.

## Prerequisites

- An OpenAI API key (paid)
- A free <https://newsapi.org> API key
- Python 3

## Setup

Create virtualenv and install dependencies:

```bash
$ virtualenv venv
$ source venv/bin/activate
$ pip install -r requirements.txt
```

Add your API keys into `.env` and source the environment variables:

```bash
$ cp env-example .env
$ nano .env
$ source .env
```

## Running NewsGPT

Start the chatbot:

```bash
$ python newsgpt.py

Hi, I'm a NewsGPT a breaking news AI assistant. I can give you news for most countries over a wide range of categories.
Here are some example prompts:
 - Tell me about the recent science discoveries
 - What are the lastest news in the US?
 - What has Elon Musk been up to recently?

What would you like to know? =>
```

You can ask questions on any topic. You can also ask about specific countries or categories. Check the [newsapi.org](https://newsapi.org/docs/endpoints/top-headlines) reference to see all available options.

```
=> What has Elon Musk been up to recently?

Working...
Processing 1 articles from newsapi.org
Working...


==Response==

According to the latest news, Elon Musk and Mark Zuckerberg have agreed to fight each other in a cage match. This news was reported by BBC News. You can read more about it [here](https://www.bbc.com/news/business-65981876).

==End of response==
```




