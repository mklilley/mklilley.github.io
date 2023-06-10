+++
author = "Matt Lilley"
title = "Back in stock"
date = "2022-10-17"
description = "I need to buy new fridge with some annoyingly specific requirements. The problem is, the fridge keeps going out of stock and the website's built in notification system is so slow that by the time I get the \"back in stock\" email it's too late...out of stock again! I couldn't resist the urge to make a little bot 🤖 to solve this problem."
subtitle="Building a stock checker and notifier 🔔"
tags = [
    "technology"
]
+++

I need to buy new fridge with some annoyingly specific requirements. The problem is, the fridge keeps going out of stock and the website's built in notification system is so slow that by the time I get the "back in stock" email it's too late... it's out of stock again 😩.

Because I like building stuff, I couldn't resist the urge to make a little bot 🤖 to go check the website for me every few minutes. This way, I'll hopefully be able to get ahead of the "crowds" 🤓.

The bot works by scraping the website and searching the page for a specific bit of text that only exists when the product is out of stock, e.g. "out of stock". If the bot can't find that text then the product is assumed to be back in stock and a message is sent to me on Telegram. 

I'm sure I'm not the only one with this problem, so if you too are suffering this first world inconvenience then please feel free to go download the code from the [back-in-stock-alert](https://github.com/mklilley/back-in-stock-alert) repo on Github and use it as you wish.

