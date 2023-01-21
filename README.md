# iro-treasurer-website

This is an empty repository with just a README file as a placeholder for the newest version of the [iro-treasurer website](https://iro-treasurer.herokuapp.com/). 

## About
This website was made by Charlie Meyer as a campaign promise to bring back financial transparency to the IRO. The former treasurer websites written by Mohit did achieve this, but required manually updating them and some features became outdated. So, at its current state, this website displays the current IRO bank account balance and recent transaction information. Additionally, another feature will be added later to also include a DPM scraper on the website as well, so that the website is finally the all-in-one hub for everything anyone would need from the treasurer.

## How did I make it?
Before this website was actually written, I first had to write a BoFA scraper, which I did in python using Selenium and Google OAuth. Then, after realizing that I wrote it in python , I then came to the sad realization that I had to write my website using some sort of python website framework, and I then landed on django since that's the only one that I have experience with (I am a react fanboy). Then, using some post/get request magic and an ungodly amount of regex, the website does what it does - displays banking information! 

Hosting on heroku was unfortunately the only option I had, as it allowed the use of webpacks that allowed Selenium and also, despite how annoying it can be sometimes, is super powerful and easily scaleable. There's a decent amount of security on the website - the code isn't public, it uses gunicorn rather than just straight-up doing `python manage.py runserver` and Heroku does other security things, as well. 

## Contact/Help further develop the Website
I'm always looking for help to make this website better<sup>[Citation needed]</sup>. Since i made this over winter break just as a small passion/side proejct, there are many features/pages that I wish i had added to the site that I just didn't - I want to make the about page an actual about page rather than just liking to the main IRO website, and I also want to make the DPM script functioning on the website. If you have any interest/skills in web development (and want a cool resume bullet point too!) hit me up - abs6bd@virginia.edu

## Credit
First of all, while the main functionality of the website was written by Charlie Meyer, he did not create the UI. This UI was from a Django template that I found online for free. I also have to shoutout ChatGPT as they were super helpful as well. I also semi-repurposed a BoFA scraper I found online, but ultimately the majority of the BoFA scraper is written by Charlie becuase the old BoFA scraper was outdated. 
