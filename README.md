# Crawl.sh

> Yet another intelligent spider.

**Note**: 
If you just want to know how to use, you can omit this page!

**注意**: 
如果你只是希望知道如何使用，这篇文章可以略过!

## Introduction
As computer technology continues to 
develop these years, more and 
more information has been published on to the internet. 
Most businesses have to be extremely sensitive to the information
published by different online information providers (like 
New York Times, etc.). However, either programming requirement
of currently available crawling system or huge cost of hiring
spider developer blocks the way of companies to gain enough 
published information. 


After massive project practice and summaries, 
Crawl.sh, an easy, elegant, online spider, is refined 
by Zwang Team. It could crawl any web page that 
you could reach by your Chrome just by a few easy 
button-clicking settings. 

If you are not a programmer, you could use our panel for
data visualization and NLP analysis. It is well-designed and
don't worry, no coding needed! Indeed, you could even define your NLP analysis
by training our model with small amount of data. (Also
no code needed) If you are a programmer and 
hope to get your hand dirty on the other hand, 
we have APIs and SDKs for data retrieval and online/offline
NLP analysis. 

## Cases
* Searching  
    Searching system requires huge amount of data on internet.
    With Crawl.sh, you could define a searching system of a 
    specific website by crawling all of their pages! We would 
    handle the coding of searching.
    

* Warning  
    We provide instant push notification. You could choose 
    to be notified at the end of each epoch or even 
    each time the webpage is crawled or changed (difference
    identified between each epoch). With this, you could 
    analyze in time and conduct a warning system.


For more information, you could take a look at 
[API Docs](en/API)

## Principal of Design
* Easy to use  
    We value our easiness of use as one of the priorities. 
    Unlike most online commercial spider system, we 
    hope that our user could crawl directly without 
    writing code. Apart from that, we grasp any chance 
    to decrease the step needed to be finished and 
    buttons needed to be clicked. Indeed, the average 
    time for setting a spider on our system is 20 seconds.

* System reliability  
    Although this is not about CRM or others, we still 
    tried our best to putting more 9s on our SLA. Here are 
    a few ways we keep our SLA works:
    1. In our system, each master server (Database/API/
    Crawling system) has two slave servers for backup.
    2. For each crash or error in the system, we would 
    take a snapshot and analyze carefully as soon as possible. 
    3. Each module of the system is weakly correlated 
    so a crash in one module would not lead to the crash 
    of the system. 
    4. All third-party module or systems used are 
    well-developed and used by millions of developers.

* Efficiency  
    If you pay enough money, the system could crawl the 
    whole Medium.com or Yahoo News in less than a minute. 
    The system is widely distributed and deployed in 
    different countries. Task would be dispatched to 
    the server that has the smallest distance with the 
    website. Also, the servers are elastic. We used 
    AWS, Alibaba Cloud, Google Cloud, and Tencent Cloud. 
    If the system determines that it is overloaded, 
    it would create new cloud servers. We also used 
    a few big-data tricks to ensure the fast delivery 
    of data through APIs. All in all, your time is 
    worthwhile in our mind.  


## Security
* E2E  
    All data between your computer and our systems is 
    encrypted end-to-end with SSL by default. Other 
    uploaded assets and backups are also stored and 
    transmitted using encrypted connections.
* PCI  
    Aparker does not store credit card information on 
    any of our servers.  Instead, we securely transmit 
    information to Alipay and PayPal, our PCI-compliant 
    payment gateway, which handles your transactions.
* Disaster Recovery  
    We have performed a comprehensive analysis of 
    risks to our business and have a Business 
    Continuity Plan and Disaster Recovery Plan 
    in place. We have warm standbys of our applications 
    and data in backup OSS.
* Liability  
    We utilize proxies to ensure the anonymity 
    of crawling clients.

If you’d like to discuss further aspects of our security 
and compliance policies for your own internal records, 
please contact us for a briefing under NDA.
## Opensource Softwares Used
Backend
* [Celery]() - For dealing the job queue
* [Flask]() - For API server
* [Requests]() - For crawling webpages
* [Redis]() - For counting epochs and instant settings
* [MongoDB]() - For saving webpages
* [ElasticSearch]() - For searching system
* [Selenium]() - For spoofing anti-spider system
* [Google V8]() - For analyzing JS
* [MariaDB]() - For saving user data
* [Zookeeper]() - [SECRET]

Frontend
* [jQuery]() - Anything!
* [gin]() - Frontend template engine

Other
* [glibc]() - [SECRET]
* [git]() - Version control for webpages in different epoch
* [docsify]() - How this is built
* [JVM]() - [SECRET]

## About Us
We are a group of geeks and hackers. For more information,
you could visit the official website of 
[Zwang](https://zwang.tech)

## Join Us
Send an Email to `b64decode("akB6d2FuZy50ZWNo")`
