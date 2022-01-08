---

layout: post
date: 2022-01-06

---
- A working notification system has been implemented with the originally intended features, but has many problems and will be heavily revised. Currently a user can input a low and high value with a cryptocurrency and be notified when the value of that cryptocurrency surpasses this high or low. If the user leaves the page the notification will be removed. Also, the input field for cryptocurrency is loosely defined and will not work if given an invalid cryptocurrency abbreviation

**There are many things to consider for building the notification system.**
1. First off, there may still be some untested logical holes that need to be fixed, such as negative numbers, and although I have attempted to divert this in my code, there hasn’t been enough testing to catch something I have yet to see.
2. Another problem is that a user can create as many notifications as they want while on the page and even create multiple notifications for the same coin. I want there to be only one notification per coin and this may be possible to implement with some logic gates and javascript objects without resorting to a possible backend implementation. Also, there will be a dropdown menu for selecting a crypto-currency and will most likely only have the top 20 most popular coins.
3. The largest problem is that of running the notification system even if the user exits the page. This is leading the front-end project into a full-stack project. In order to store each unique user's specified input data there will need to be a database connected to some server side programming language. For this I will use MongoDB and Node.JS and want to try out some typescript as well. What will allow this to be possible in the first place is something called a service worker, something I do not know too much about and apparently was introduced only in 2016. 

- Before the full notification system is built I will put in a simple Alert box to notify the user that it will disappear upon leaving.
- Additionally, the graphs have been updated since upon realizing the data disappears when viewing the notification page; now the user will see the displayed history and a point will update reflecting an interval past the time when the user entered the page (so if the interval is 5 minutes, upon entering a data point will emerge after 5 minutes of the price of the coin along with the date). 
- The UX and design of the website has had little attention and is hardly or not at all accessible by phone yet. Next time the mobile first approach should be used. I hope to have made serious improvements to the UX of the site by the time of the next update.