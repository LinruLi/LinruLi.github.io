---
title: Next Generation Networked Hardware Project
featured: /assets/images/pic06.jpg
layout: post
---

# On-boarding Documentation with design choices


**Backend Code**

The code is all written in Java. There are four folders in &#39;src&#39; which are bean, db, servlet and utils. bean folder contains two files, those two files are used to encapsulate feedback information in Json. This can be seen as a necessary part to get Json feedback working after Pi making an HTTP call to the server. DBUtils file in db folder means to handle all connections to the MySQL database. Therefore all queries were made there which was to grab the information you want from the database. And obviously, the file in servlet folder manage to deal with all HTTP request from the Raspberry Pi by calling methods provided in DBUils, which then get the row, column and image code stored into the database. In utils folder, Base64Utils here is to decode the code and generate the image in term of the coming in the request. TimeUtils class is able to generate time stamp and append to the end of file name just for a testing of the updated image does get stored into the right folder at the very beginning. TokenUtils is just to combine values of pantry row and column used as a token symbol and show them into the Json feedback.

Since all code was written in Java that means at which it gets to the moment of deploying on a server somewhere, make sure you have installed Java library and MySQL database first. Additionally, there are two dependencies were necessary needed in the project: Gson library and JBDC(Java Database Connectivity).

For running this backend in different IDE, pay an attention that on Eclipse, only run the UploadServlet file would bring the server up; On Intellj, add a Web module on the left panel and then build, then the project would get connected with the server.

**Database**

You might notice this project also required a database. The schemas named Login and it included one table named userinfo. In the tables, image\_id is its primary key and set up as auto-increment value. The pantry\_column and pantry\_row are two attributes that contain extracted values from the HTTP call from row and column respectively. The image\_code contains a path information of that corresponding generated image which stored under a folder specified in the code previously. The last attribute is token. As said before, it simply stored a combined values of the row and the column, which might be useful for future use.

**Future functions assume**

Because I had a fully functioned database charging all information storing, it would then get fairly easy to retrieve them. For the frontend bit, we have not included any archive function that enables the user to browse through old photos. The TimeUtils provided already may become handy to use to accomplish the feature.

**Platform Chosen**

Chosen Java as my backend code became my first choice because of its great compatibility with all platforms. We separate the front-end web and the backend database into two different frameworks since Django is good at handling pictures. Java backend is sophisticated for handling HTTP Request and Response. Have them separately was so much easier for debugging the server problem at some point.
