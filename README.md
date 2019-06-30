#### This is a fork from the original founders and coders repo, to use fetch instead of XHR requests in the solution

# workshop-APIs

In this workshop we'll build on things we've learnt so far by using the GitHub API in order to practise:
- Making HTTP Get requests on the client side
- Using the Fetch api
- Working with large amounts of JSON-formatted data
- DOM manipulation

**Mentors** see [notes.md](https://github.com/emilyb7/workshop-APIs/blob/master/notes.md).

## Remember
Pair programme!


## Getting started

1. Clone this repo and open in your text editor

2. Open index.html in your browser. You'll find a template with space for some info which you can find on your GitHub profile.


## GitHub API

You can find the API docs [here](https://developer.github.com/v3/).

You can make calls to the GitHub API without an API key. However, the rate limit for _unauthorized_ requests is quite low at 60 calls per hour (per IP address).

To increase your rate limit you can [create an access token](https://help.github.com/articles/creating-an-access-token-for-command-line-use/). When you get to the screen that asks you to _select scopes_, you don't need to select any additional scopes.

**Note that this is NOT good practice: access tokens (which are not the same as API keys) should always be kept private and never, ever pushed up to GitHub! Use your access token for this workshop only and do not share with anyone else**.

Once you've got your access token, you can add it to the URLs you call like this:

`https://api.github.com/users/octocat/orgs?access_token=YOUR_ACCESS_TOKEN`

Try and complete Task 1 with at least 2 tests and don't rush ahead to the challenges. This is the most important part of today's workshop. The other parts should be treated as extra challenges.

## Task 1 (45 mins - 1 hour)

Use everything you've learned about APIs and callbacks to make a call to the GitHub API that gets details of _your_ GitHub repos.

Use the response to populate your HTML template down to the horizontal line.

You don't have to stick to the template I've prepared for you. By all means, you can choose to show different data from the API and to present it any way you like.

-----

## Challenges (one hour, longer if teams finish the above quicker)

Have a go at one (or more) of the challenges below. Do pair program! You may have to do a little bit of independent research. At the end of the session we'll expect all pairs to present for 2-5 minutes.


### Challenge 1.0: make another API call

Go back to ```index.html``` and un-comment the commented-out HTML below line 30. This is for showing of details of one of your repos. It can be the first repo in your list, the last, the most popular, or whichever one you like.

How could you go about getting the relevant data from the GitHub API? Refer back to GitHub's documentation for help.

How might you have to adapt your code from the first exercise?

Try and at least come up with an **idea** of how you might do this. It will be very useful when you come to your end-of-week project!

### Challenge 1.1: even more API calls

What other data might you want your application to show and what API calls would you need to make?

Do the structure of your code (after challenge 1.0) allow for you to easily accommodate these changes?

What problems can you foresee?

### Challenge 2: adapt your app for different users!

At the moment, your app is just getting data about one GitHub user. But what if you wanted to use it to compare everyone from Founders & Coders? Or to get data about a custom GitHub user? How might you adapt your application for this purpose?

Try and sketch out a plan!

-----

## Presentations

Prepare for a quick 5-minute presentation in pairs on your findings!

## Solution!

There are many ways to go about this challenge. To see a working solution (to part 1 + challenge 1) pull down the branch "solution" and check out solution.js (and the tests!).

Disclosure: it took me much longer than 2 hours to perfect my solution!
