---
layout: post
title:  "My First Project :D"
date:   2017-02-12 04:11:51 +0000
---


Today, I have just finished (and will submit for review) my very first programming project! For this project, our task was to build an Object Oriented Ruby application that provided a CLI to an external data source.

### Coming Up with an Idea

When I first looked at the CLI Data Gem project instructions, I was really unsure what I should do. I thought of hobbies that I loved and things I liked to do -- baking and traveling stood out the most to me. So, I spent some time looking online for travel blogs or top places to travel. I also looked at different websites related to baking and food. However, none of them really stood out to as websites that I wanted to base my entire project around.

After much time spent thinking of an idea, I remembered how much I wanted a pet, and thought it would be a great idea to base my project around animals. That is when I found the WWF's Endangered Species List and decided to run with this project idea.

 ### Step 1: Basic Structure

When first tackling my project, I spent a lot of time in the beginning deciding how I wanted to structure my project and CLI output to the user. I ultimately decided that I wanted to structure the CLI output as follows:

* The user will be greeted with a Welcome message.
* The user will be asked to choose which conservation status they would like the program to list animals of (1. Critically Endangered, 2. Endangered, 3. Vulnerable).
* Based on the user's input, the program will list the animals of the chosen conservation status (listing the name and scientific name).
* The user will be asked which of the animals they would like to learn more about. Based on this input, the program will print a description of the animal (name, scientific name, status, population, habitat, places, description.
* The user has the choice to see another animal (and repeat the process) or exit the program.
* The program ends with a closing thank you message.

### Step 2: CLI and Animal Class 

I started my project with a CLI class and an Animal class. I worked in the CLI file to come up with the basic methods I would use to run my CLI and print out the data after it is scraped. I used fake data at first in order to test if my CLI was structure was working as I planned.

Once I got that working with hard-coded data, I working in the Animal class to get and scrape real data from the website. (Originally, the methods I had in my program to scrape data from the website was stored in the Animal class and used to create Animal objects and add information to those objects. I later moved the scraping methods to thier own Scraper class.) 

I started writing the method to scrape the first level of data for my program. This data lists the animals on the website (name ad scientific name) based on the user's input. So, my first goal was to be able to scrape ALL the animals from the website (whether or not they fit the chosen conservation status). I used ./bin/console and Pry a lot while I trying to figure out the best way to scrape data. Eventually, I was able to scrape the correct number of animals, but I ran into a huge problem where the program output the same animal (name and sci. name) each time! With some research and trial/error though, I was able to fix this problem and scrape the animals nam eand sci. name correctly. I then worked with my program to output ONLY the animals whose conservation status was chosen by the user.

After I got the first level of my program to work, it was time to tackle the second level. This level of my program scrapes additional information of an animal based on the user's input. With this level especially, I used my console and Pry A LOT in order to scrape the information I needed successfully. Once I got the correct information to print out, I had a working (but not too pretty) program.

### Step 3: Formatting, Validation, and Scraper Class

Throughout the whole time writing my program, I was constantly updating how I wanted the CLI output to look. I spent a lot of time formatting my output and making sure that it looked nice with .ljust() and .rjust().

I also had a lot of code that verified the user's input and made sure it was valid. I started writing this code from the beginning, but I was working on perfecting it until almost the very end of my project process. Near the end of the process as well, I separated the different sections of input validation to their own methods in my CLI class so I could clean out my main 'start' method.

One of the last things I did with my program was separate the methods that focused primarily on scraping (originally in my Animal class) to thier own separate Scraper class. I realize I should have done this from the beginning, but I was in the zone getting my program CLI to work and I was not sure at first how to implement these methods in their own Scraper class. With some research and testing, I was able to successfully move the methods I needed to in this class and update the rest of my program to reflect this change.

### Step 4: Last Minute Changes / Bugs & Comments

The last things I worked on in my project were adding comments to all of my methods and perfecting some bugs in my Scraper methods.

###Comments

I really wanted to add comments to my program because I thought it would be great practice for me. Because most of my labs are test driven, I don't normally write comments for them. However, I felt it would be helpful for me in the future to have comments in my project in case I need to update any information later or fix anything. It also can be helpful for others trying to understand my code.

###Bugs

Although I ran into bugs throughout my project process and fixed them, the last bugs that I took the time to fix were a few things that I had been having trouble fixing from the beginning. 

1. The descriptions I scraped joined paragraphs without a space in between.  I really wanted the output in my CLI to be perfect, so I ended up debugging this with Pry and finally figured out that I just had to make one simple edit to how I scraped my descriptions and add .gsub to replace "\n" with a space (" ") instead.

2. I was having trouble scraping habitat correctly. I had noticed that when there was not a 'place' and there was only a 'habitat' listed on the WWF website, my code did not scrape the correct habitat data, and had it as [Unlisted]. I decided to scrape the 'place' data as well and add this to my CLI output and Animal class because I felt it would be interesting information and I could write a few conditional statements to scrape both habitat and places correctly as their formatting on the WWF website worked hand-in-hand. (Originally I did not decide to scrape 'places'.) This took me a few hours to scrape correctly, but thankfully I managed to fix this bug!

### Closing Remarks

Overall, I am very excited to see everything I have learned in the past few months work together and come to life! This first project has been a challenge, but has taught me so much about writing good OO Ruby and practice coding in general. It also taught me how useful Pry is in testing and debugging my code -- I will definitely use Pry more in the future.

Thank you for reading~! :D
