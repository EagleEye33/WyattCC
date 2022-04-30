---

layout: post
date: 2022-04-30	

---

- after a small hiatus the website has had notable improvements. Many of the client side issues have been solved, but still no user will receive a notification upon leaving the notifications tab. This part of the project (and part of the reason for the hiatus) is that implementing a service worker involves a lot more than anticipated...
First here is a list of what has changed since the last update
1. No logical loopholes or errors have been found in the notification system.
2. A user can only have one running notification at a time: no more possibility of making a thousand notifications. Also, there is a dropdown menu with three predefined values, not twenty as planned (maybe in another update I will add more to the dropdown)
3. There is no alert box added to the notifications page upon leaving; I have decided to just attempt to go straight to builidng the service worker (although adding an alertbox would be easy, I decided it isn't necessary)
4. Currently the historical data for the cryptocurrencies is in increments of hours
5. The UX of the website has improved and a logo was added

- Now I will be focusing on the main development of the website: implementing a service worker. So far I have had to spend time learning how to create a backend with Node.js, Express, MongoDB and Typescript that registers a service worker and sends a push notification. I can say I have learned a lot in this regard and will now be moving on to Amazon Web Services to host the site and backend. Another update will launch once the site is hosted and hopefully there will be a service worker script by then that sends a simple web push notification to users who subscribe to a notification.     