---
layout: post
title:      "My First CLI Project"
date:       2020-09-13 20:33:01 +0000
permalink:  my_first_cli_project
---


This project was a great challenge for me in many ways... and not all of them were coding related! 

When I learned about the nature of the project and how I was going to be working on this, I originally started off with planning out my week and what each day would entail. Monday, I planned out the schedule of my program and what specific parts I would want to work on. I did research and found everything I needed to complete my project. The API I wanted to use, the name of the program and its design, what it would accomplish... I was off to a great start.

Then Tuesday happened. I learned that a lot of what I wanted to accomplish was incredibly ambitious and would take far more time than I had estimated. I started to cut back a lot and restructure my goals to be more reasonable and something I could accomplish. I can't lie, this was a time of great stress... I had thought my goals were fine until I started working towards some of the more complex and difficult challenges. It's not easy to admit when you're wrong about something, but it was something that I needed to acknowledge.

Wednesday was the worst for me, however... I ended up losing a good portion of my project because I forgot to save what I had worked on. It was depressing and felt like I was moving backwards instead of fowards. Much of what I had created wasn't very complex nor difficult, more amounting to a simple framework that needed filling in. I didn't accomplish much due to the setback... but it did give me the breathing room I needed to rethink my strategy. I was tackling this in an unproductive way.

Thursday is when things began to swing upwards! I finally understood what exactly I was going to work towards and began to structure what my API program would do.  Instead of a super complex set of logic that would organize data as it was recieved, I opted instead to simply recieve the data and pass it to a class that would organize itself.

class API

    def self.scrape_account(apikey)

        resp1 = RestClient.get("https://api.guildwars2.com/v2/characters?access_token=#{apikey}&page=page=0")

        char_hash = JSON.parse(resp1.body)
                            
        resp2 = RestClient.get("https://api.guildwars2.com/v2/account?access_token=#{apikey}")

        account_hash = JSON.parse(resp2.body)

        Account.new(account_hash, char_hash)
    end

end

Using this class, I was able to create a main table class (Account) that would distribute data to other classes as its generated. This let me organize the objects into the Account class itself for later use. Finally I could feel a big breakthrough in understanding how I got information and then organized it.

Friday was a blur of work. In retrospect, I should have saved more often to show where my work had improved and the changes I had made instead of simply saving every hour or so. A lesson learned from working on a project like this for sure. A large part of this day was spent working and reworking the data I had recieved into a readable format for my user. After all, a program that is hard to understand is not a very good program for a user. My goal was to create something fun to use while getting exactly what you wanted.

Saturday saw the completion of my Account Dragon program. It's not nearly as ambitious as I had wanted it to be (and I plan to add more and refine it in the future as a personal project!) but it had accomplished its starting goal. The lesson I learned from this project was that I need to start small and grow outwards. Don't try to accomplish everything all at once and tackle your problems one at a time steadily.

It was a fun experience. I had never built a program from scratch like this before... it gives me a great deal of respect for people who create elegant software for a living and makes me excited for the future of my own development career!
