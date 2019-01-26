[![Build Status](https://travis-ci.org/susanx/whotube.svg?branch=master)](https://travis-ci.org/susanx/whotube)
[![Build Status](https://travis-ci.org/susanx/whotube.svg?branch=master)](https://travis-ci.org/susanx/whotube)
[![Coverage Status](https://coveralls.io/repos/github/susanx/whotube/badge.svg?branch=master)](https://coveralls.io/github/susanx/whotube?branch=master)
[![Code Climate](https://codeclimate.com/github/codeclimate/codeclimate/badges/gpa.svg)](https://codeclimate.com/github/susanx/whotube)

![](https://i.imgur.com/95LeuJ1.png)
# Mike, Susan, Alex, Lucy 

### About 📝
Founders and Coders is a 16 week coding BootCamp. Every week (for eight the first eight weeks) students are asked to complete numberous workshops/challenges around a specific web-development subject.
These workshop/challenges are created to stretch and challenge students knowledge which means they are often started but not completed.

WhoTube is a mobile-first web app for those who want to keep their favourite youtubers' latest videos and tweets in one place, always under control!

## Setup instructions :books:

Geeky version:

* ```clone``` the repo
* ```npm i``` 
* ask us for the keys!:key:
* ```npm run dev```
* go to your on ```http://localhost:5000/```

or more simply, &nbsp;
- navigate to https://whotube.herokuapp.com

## Prototype
![](https://www.dropbox.com/s/9hn05qxzitj32ct/figma.png?raw=1)


## Logo ideas:
Whooootube! The owl idea came out quite randomly, but we liked how it sounds.
![](https://cdn.dribbble.com/users/20931/screenshots/2518827/trivify_g1_dribbble.gif)

## User stories :eyeglasses:

1. As a user, I want to be able to enter a youtuber's username and see their most recent videos.
2. As a user, I want to be able to see their twitter too.
3. As a user, I want to see the text and the video large enough to be read and watched.
4. As a user, I want to be able to refresh the page in order to see if the youtuber I follow has updated their profile.

## YouTube API 

* We overcame quite complicated documentation to successfully retrieve the data we wanted.
* Through a nested list of 3 API calls we can:
    1) retrive the Channel ID for a selected youtuber,
    2) then look for the playlist,
    3) finally the latest videos.
* We worked in order to make sure the search function would be able to interpret the user input in most cases. 
Should the word that the user input lead to partial or any result at all (e.g. youtube and twitter accounts have different names), the user will have che chance to manually add youtube and twitter user names in two dedicated searchboxes.

## Twitter API

* Starting from the same inpout search, unless the youtuber had a different name for their twitter account (see above), the latest 10 tweets will be displayed alongside the latest videos.
* We added date and time to the tweets in order to make it easier for user to tell most recent tweets from the least.

## Usage instructions

1. Type your favourite youtuber in the searchbar;
2. If the name you typed is successfully found on both YouTube and Twitter, you will see a page displaying the latest 4 videos and 10 tweets of the youtuber you search for.
3. Should the person you typed have a differently spelled twitter name (it happens often, as twitter uses one word usernames) you will be given the chance of searching for both YouTube and Twitter names in two separate boxes.
4. Enjoy WhoTube!

