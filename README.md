# Content on X

This repository contains the content that has been posted on X (Formerly twitter).

## How to post

- Include a file with extension `.tweet` in the `tweets` folder.
- If the tweet contains images, include them in the `media` folder and reference them in the tweet file (explanation below).
- Create a PR and the tweet will be posted when the PR is merged.

## Recipes for tweets

Copy and paste one of the following examples into your `.tweet` file to quickly get started with a tweet.

### Simple Post

This creates a simple tweet with only text, just throw the text in the tweet file.

```tweet
I love to code! #javascript #typescript
```

### Post with images

If the tweet contains images, include them in the `media` folder and reference them in the tweet file.

```tweet
---
media:
  - file: cat.jpg
  - file: dog.jpg
---

Here are some cute animals!
```

### Poll

```tweet
What is your favorite color?

( ) Red
( ) Blue
( ) Green
```

### Reply

If you want to reply to another tweet, include the `reply` item with the tweet link that you wish to reply to.

```tweet
---
reply: https://twitter.com/whatever/status/1409601188362809349
---

@whatever I love your work!
```

### Quote

If you want to quote-retweet another tweet, include the `retweet` item with the tweet link that you wish to quote-retweet.
If you'd prefer to just retweet without quoting, don't provide a tweet body after the the `retweet` item.

```tweet
---
retweet: https://twitter.com/what-ever/status/1409601188362809349
---

quote-retweet is awesome!
```

## Initial Setup

Go to [initial-setup](docs/initial-setup.md) for instructions on how to set up the project.
