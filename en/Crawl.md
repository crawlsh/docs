# Setting of Crawling

**Note**: This document describes how to set a crawling
job. 

## Crawling Methods
To begin with, you have to tell the spider where to crawl.
Don't panic, you do not need to input links by hand. Choose
one of the following!


**1. Crawl by templates**  
You could search the name of website in the homepage 
of our system. If there is a match, congratulations, 
you could now crawl by the template! Just follow it’s 
clear instructions.  

**2. Crawling by patterns in link**  
Suppose you want to crawl articles from a news 
website and you observed that the link of each 
article is like following:
```
https://news.com/article.php?id=5
https://news.com/article.php?id=6
https://news.com/article.php?id=7
...
https://news.com/article.php?id=127
```
You should see the difference. Each article link 
is differed by the number at the end. Then,
this website is a perfect fit for crawling by this 
method. You can now follow the instruction on Aparker.  

**3. Crawl everything**  
Well, it is disastrous and is the worst method 
for crawling. Unless your website does not 
fit foregoing methods, do not use this method. 
It is slow and not promising. However, it is easy 
to work with the setting of this method. Try it 
on the Aparker.  

## Select the content you need
You need to select some texts on the webpage so that 
we could know what you want. 

**Case 1: The crawling template lists what you can crawl**

Just click whatever you want!

**Case 2: You need to select what you need in the browser**

By clicking directly on the webpage, you could 
see a popup window. Follow the instruction there. 

**Note**: You need to be careful on determining if 
you click the whole text or just the first paragraph.

## Definition
Things you do not need to know unless you want to
learn about the mechanism behind.

**Epoch**  
Each performance of crawling everything you want is an 
epoch. In each crawling job you submitted, you can either 
choose to have only one epoch or multiple epoch that 
executes at different time.

**Template**  
A template is a module that has already been developed 
by our crews. It helps optimize the crawling job. So,
if this option is available, choose it without hesitation.

**URL Template**  
Don't confuse it with template. It is like a generator for
links. You may not configure it in common cases. If you hope
to configure it, here are a few conventions:
```
@{integer 1}
@{string 1}
```