# Your Little Pony

Your Little Pony is a collection of My Little Pony screens from Season 1 and Season 2. Plus some scripts, which help you post those screens wherever you want.

## Why?

Why not? Ponies are cool! Pinkie Pie is the most awesome of all! So tell me why not?

If you need a justification, though. I know that the developers in my team work really really hard. Unfortunately, the immense brain activity always results in huge amounts of stress. Ponies here are a "comic relief", a coping mechanism to relieve tension and reduce the amount of stress everyone is experiencing.

I have a Slack app, which posts to #pony_of_the_day channel three times a day, saying "Good morning" at 9am, asking if the channel members had already had a lunch around noon and wishing the perfect rest of the day at 5pm. I hope this brings a smile to the members of #pony_of_the_day and they feel a little bit better every time they see a pony.

## Installation and Usage

Installation is siple. Do `git clone` and you're ready to go.

Right now there is only one script, which posts to Slack.

## Slack

You absolutely must create and configure a Slack App before you can post images to Slack. A good starting point is [Your Slack Apps](https://api.slack.com/apps), the rest is in their documentation, please refer to that.

Then you must copy `slack.config.dist` to `slack.config` and manually set up all the values.

The `slack` script has only one optional parrameter, which is the image comment. If you do not provide one, then the one in `CONFIG[message]` is used as fall back.

```
[akarshin@localhost yourlittlepony]$ slack                                  ### This will send the defaul message, which is "Pony Of The Day!"
[akarshin@localhost yourlittlepony]$ slack "Good morning!"                  ### This will send "Good morning!"
```

After you're done with installation, you can set up cron, which would call `slack` script, for a bit of automation. Otherwise you'd have to run the script manually.

#### How does it look on Slack?

![View in channel](https://i.imgur.com/Jdco2La.png)
![Detailed view of uploaded file](https://i.imgur.com/K20DMmD.png)


## Disclaimer

My Little Pony, all images, animations, characters and other works are trademarks of Hasbro, Inc. © 1999 Hasbro, Inc. All Rights Reserved. However, I use it solely for non-profit non-commercial activities, but rather for comment and/or criticism in insignificantly small quantity with absolutely no effect on the market or potential market for copyrighted work with restricted access to an appropriate group, which would be considered Fair Use according to Copyright Law Section 107 (and possibly other) of the US Copyright Act.

The MIT Licence this repository uses is applied to everything, but the copyrighted works described in the previous paragraph, the code, documentation and other.
