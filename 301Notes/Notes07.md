# Code 301 Class 07 Reading notes:


## How I explained REST to my brother 
The whole world wide web is built on an architectural style called “REST”. REST provides a definition of a “resource”, which is what those things point to.

### Who is Roy Fielding? 
Some Smart Guy..



### Why don’t the techniques that we use today work well when we need to be able to talk to all of the machines in the world?
Because they weren't designed to be used like that. When Fielding and his colleagues started building the web, being able to talk to any machine anywhere in the world was a primary concern. But most of the techniques developers later used to get computers to talk to each other didn't have those requirements. You just needed to talk to a small group of machines.

### What is the HTTP protocol that Fielding and his friends created?
HTTP—this protocol Fielding and his friends created—is all about applying verbs to nouns. For instance, when you go to a web page, the browser does an HTTP GET on the URL you typed in and back comes a web page.

Web pages usually have images, right? Those are separate resources. The web page just specifies the URLs to the images and the browser goes and does more GETs using the HTTP protocol on them until all the resources are obtained and the web page is displayed. But the important thing here is that very different kinds of nouns can be treated the same. Whether the noun is an image, text, video, an mp3, a slideshow, whatever. I can GET all of those things the same way given a URL.



### What does a GET do?
Retrieve Data
### What does a POST do?
Create Data
### What does PUT do?
Update Data
### What does PATCH do?
Partial Update.


## API Keys

Request a personal API key from the following APIs. You should receive these in your email within a few hours, often within minutes. Please request these keys prior to lecture to allow adequate time because you will need them in order to complete your lab assignment. Note: do not post your API keys in the Canvas discussion or on GitHub. Save them in a secure place.

### Geocoding API
#### Did you get your API key?

Yes

### Weather Bit API
#### Did you get your API key?

Yes

### Yelp API Docs
#### Did you get your API key?

No 

### The Movie DB API Docs
#### Did you get your API key?

No




## Things I want to know more about


#### Want To Know More ? 

[REST](https://gist.github.com/brookr/5977550)
