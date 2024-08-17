# 👔 Scrapping Linkedin - Schulich CCD Activity Posts

Code I created to scrape Linkedin CCD for Schulich networking opportunities, feeding into my "Schulich MMAI Network Cheatsheet" Google Sheet.

The Google Sheet, designed to help Schulich MMAI Students find networking events, can be found [here](https://bit.ly/mmai_networking)!

PROBLEM:

- It was observed that, while the Schulich School of Business does offer information regarding networking events on their internal platform "Handshake", that it would often require tedious logging in and if a student wants to track the information, it's difficult and manually time consuming to complete.
- Additionally, the email notifications sent to Schulich students is often later in the week or month, on versus immediately after the opportunity is posted on the Linkedin platform.

SOLUTION:

- It was observed that the social media team for Schulich CCD is often more timely and rapidly updating the Schulich CCD Linkedin page with the new opportunities.
- Given how this is publicly available information, and as a Schulich student/Alumni, it would be a great exercise to practice scraping online using Python, Beautiful Soup and Selenium.

THE PROCESS:

- Installation and setup of Chrome Drivers, Selenium and Beautiful Soup
- Saved Chrome profile and cookies connected to a Linkedin account, used for scrapping
- Successfully able to scrape Linkedin posts
- Determine the "pattern" to the social media team's posts - i.e. using emojis and references links (app-aware-links) in their HTML structure of classes.
- Extracted each post and the strings associated with it, cleaning each string to remove redundant information in the process
- While not perfect, it does significantly reduce the amount of time for the Sheet Owner (me, Christine) in terms of time updating the Google Sheet. Currently, I tediously and manually write down the name, event date, location, and hyperlink the registration webpage, but the Linkedin page has this information already.

LIMITATIONS:

- Based on human observations of post patterns from Schulich CCD Social Media Team. If they change format of posting events, the code may no longer work.
- Based on last 3 months post observation, this is unlikely.
- The extraction is meant to reduce the amount of time for myself, Christine, to update the Schulich MMAI Program networking Google Sheet.

FUTURE + NEXT STEPS:

- Explore having this as a scheduled Python script, likely exploring Amazon Lambda, to complete this in the future (as students have free tier access).
- This would complete the process of establishing a pipeline.
