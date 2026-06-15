Burp Suite is an integrated platform for performing security testing of web applications. It includes various tools for scanning, fuzzing, intercepting, and analysing web traffic. It is used by security professionals worldwide to find and exploit vulnerabilities in web applications.

- it captures and enables all http/https trafffic between a browser and a web server
- burp Proxy : you capture requests between the user and the targer web server. After you capture it, u can process it by using other tools

U can intercept the traffic using proxy and block it from arriving to the web server, or you can choose the option INterception is on to allow it to arrive to the web server and continously allow requests to pass through the proxy

I configured burp proxy uusing foxyproxy in firefox. I forwarded the requests to the webservver to allow the client to access the server.
I had to check every link on the home page of the webserver, It was easier if I turned off the proxy so I wont intercept the traffic and then forward it. After that I looked at all the entries in the site map subtab in the Target tab and checked for anything suspicious in the endpoints. 

Using scoping u can select what gets proxied and what not.
  
