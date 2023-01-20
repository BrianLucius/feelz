
# Feelz Social Sentiment Tracking

This is my capstone project for the Coding Dojo Java stack. 

After earning a Black Belt on my Java Stack exam (indicating mastery of both core and advanced concepts, demonstrating the ability to synthesize new concepts under time constraints, as well as deploying the completed exam to an AWS EC2 instance), ninjas are allotted no more than seven days to design, plan, build, publish, and present a full-stack web application to their cohort.

For my second full-stack application, I created a two-part social sentiment tracking application called Feelz. The concept is for visitors to the application to rate their current mood, from sad to elated and provide a single word which describes their emotion. For their contribution a bubble chart is presented showing the relative trend of key words over the past 24 hours.

Cookies are used to prevent the spamming of the application, requiring at least 5 minutes to have elapsed between each submission. Location services for the users device and/or browser are queried (if enabled and permitted) so that each submission can be tagged with latitude and longitude coordinates for later data analytics.

The second half of the application incorporates my extensive background in data analytics. A "hidden" admin portal is available which offers fundamental analytics on the collected data, including location data, if enabled when a "feelz" was submitted.

## 👾 Tech Stack
[![My Skills](https://skillicons.dev/icons?i=java,spring,mysql,js,jquery,html,css,bootstrap)](https://skillicons.dev)  
The application is built in Java and Spring Boot. The backend is a relational database running on MySQL. The BCrypt library was used to encrypt at rest the passwords for the users of the analytics portal portion of the application.

A very basic API was created providing two resources.
* The first path returns a list of the trending emotions from the database. The list was then passed to the front end where the D3.js Bubble Chart library renders the list of submitted emotions.  
* The second path returns a list of the latitudes and longitudes of the submitted feelz and are provided to the Google Maps API for location rendering in the analytics portal.

Formatting and styling is accomplished with the [Bootstrap](https://getbootstrap.com/) library

## 🍿 Demo
* The public facing portion of the app was previously available at feelz.cc and was hosted as a droplet at DigitalOcean.  
A video of the feelz.cc app is found [here.](https://youtu.be/h05iwgrIGwI)  

* The private analytics portal, while hosted in the same location was available at at feelz.cc/analytics_portal.  
* In addition to data analytics, a user management interface is incorporated to manage the list of data analysts allowed to interact with the saved data.  
A video of the analytics portal is [here.](https://youtu.be/Rb318j61OX8)

## 🙏 Gratitude
Tremendous gratitude to [Heidi Chen](https://www.linkedin.com/in/heidi115/), my instructor for the Java stack. Her enthusiasm, passion for teaching, and in-depth knowledge of Java and Spring Boot made for a truly fun and successful learning environment. 

## 🔗 Links
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/brianjlucius)




