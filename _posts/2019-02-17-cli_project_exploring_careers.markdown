---
layout: post
title:      "CLI Project: Exploring Careers"
date:       2019-02-17 05:48:36 +0000
permalink:  cli_project_exploring_careers
---


 The process of building a CLI gem was definitely a journey. It was fun and I learned a few things as I worked through different obstacles. 
 The first issue I encountered was deciding what I wanted to.  There are so many options and range of interests so it was difficult to narrow it down to one thing. In the end I wanted to pick something that would be useful and interesting for friends to use as I developed it and had them try it out. I initially decided to build a CLI gem for world recipes by cuisines.
 This was based on the All Recipes website and it welcomed the user with a menu of world cuisines. Upon the user selecting the cuisine they are interested in, a list of specific categories for that specific cuisine is displayed. Then upon user selecting the food category they want, the screen displays a list of recipes. Once the user selects a recipe they are interested in, details for the recipe serving size, cooking time, ingredients and instructions are given. 
 
 The process of creating a basic working CLI for this was pretty smooth. I followed the pattern used in the walkthrough video for building "daily deal" CLI gem. I began by "faking" the data and went through the process of creating methods and classes needed to create the full structure of the code until all I needed to do was fill in the "fake" data with actual scraped data. I went through that whole process failry smoothly and at the end had a working CLI that pulled data from an external source. 
 
 From here I had different people run the application and give me feedback as far as clarity and information they would like to see. Then, I ran the application myself multiple times to try and find any bugs. I tried the different options I had given the user such as going back to see a previous list, inputing an invalid response, and exiting the program. I found multiple bugs and addressed each one at a time. Next, I looked through the code to make sure it was simple, clean and each class had seperate responsibilites. I noticed that I gave scraping resonsibilites to the CLI class and even the Recipe class. I tried addressing this issue using similar coding techniques that I learned from the Student Scraper lab. It seemed to be working fine until suddendly I kept comming up with an error: Connection reset by peer (Errno::ECONNRESET). After some research, I learned that many websites don't allow certain data to be scraped from their website or require a crawl delay. Because of this I actually was not able to continue scraping from the AllRecipes website. I learned about "robots.txt" to determine if a website allowed scraping or not. I used this to search for a new adequate website, however, I came across alot of sites that either didn't allow scraping or were inconsistent in the layout for each recipe. After much searching for a site to scrape, I realized these recipe websites posted recipes based on users who submitted personal recipes to their account. Because it is personal user accounts that post their recipes, many of the sites restrict scraping user info including their postings. 
 
 I decided it was best for me to change my project to something that didn't require users data but still relevant to people in my life: learning about different career occupations. I quickly found a website (US Bureau of Labor Statistics Website) that allowed scraping and was consistent in their layout. I took the same structure and code for the recipe CLI and adjusted methods, classes and variable names to match the new career profile CLI. The CLI displays a list of careern interest from which the user can pick one. Then a list of occupations for that career interest is given. The user can pick one of these occupations to get more detailed info such as average pay, education required, job oulook and key responsibilities. 
 
 The last step of the process was going back through all of my code to find any anti-patterns that could be refactored. I used the student refactoring example videos as a guide and was able to clean up my code a lot more. One thing I learned was the difference between #each and #collect. I didn't realize my understanding of these methods was incomplete. But through that process I was able to catch when I used sandwhich code with the each method. The collect method defintiely makes the code alot cleaner and easier to read.
 Another thing I learned was how to implement a find method to replace the array index logic in the CLI. This way the CLI class does not have to deal with responsibilities other than buidling a cli. Part of coding is not just getting it to work but also having clean and clear code. 
 
 I can't wait for the next project!
 
 
 
