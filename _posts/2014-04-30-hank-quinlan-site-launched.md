---
layout: post
title: "Hank Quinlan, Horrible Cop, Launches Site"
date: 2017-06-15
---

Evidence Portfolio

Evidence and Reflective for Project 1

Linru(Victor) Li - 2017/5/20

RESTful API and Django Framework

Understanding and Difficulties

Django Framework is a free, scalable and modular framework using by more
and more developers and also getting more popular among a big range of
web frameworks nowadays. Our group started our first task by using it
and its RESTful API framework trying to deliver a API that contain and
serve information for Botanic Garden visitors with the intent of using
Botanic Garden Path Mapper Android Application.

Get Familiar with RESTful API by starting with .Net API library

Our project group firstly using .Net library to grasp RESTful API in a
easier way by building up a C\# application to grab user input from its
provided search box, when user click search button it will send user’s
query parameter within a URL(http request) to Digital NZ’s API, and then
getting response back with some raw JSON data for parsing straight after
it, end up with showing a human readable data in the search feedback
form.

It was a bit tricky to filter out which one to use in .Net libraries
since there were a large amount of them available for doing this same
action. And unfortunately I was mistakenly choosing a wrong one called
‘[*ASP.Net*](http://ASP.Net) Web API 1.0’, which was too complex for me
to get through all its provided class, so quite stumbled me along the
way to send a proper http request at very beginning, then I tried to ask
help from one of my group member Andrew and he helped me with finding a
real understandable http class from the library called ‘HttpWebRequest’
that basically wrap up everything useful to properly send a http request
to Digital NZ API.

Additionally, peer programming was also played a important role through
this part of task when we tried to set up dynamic Image in one column of
a grid view within C\#Application. Me, Andrew, and Matt were able to
save big amount of time than work separately on each of our own by just
following the step provided by MSDN documentation to build up a data
GridView together and customised one column to show Bitmap image rather
than normal text.

*Evidence: Botanic Gardens folder located on CommSoft Prod Branch*

By those practices that played around with RESTful API in .NET, it gave
me more general ideas on what is it. To my understanding, it could
basically described as a URL that is able to located the query resource,
and use http verb(GET, POST, DELETE, DETC) to describe this upcoming
process, so with all these which made me feeling more confidence working
with actual Django RESTful API framework in the next.

Jump into Django Framework

Django framework provided us a more consummate experience with its
Model–view–controller (MVC) architectural pattern, but I found it was
also tricky to grasp it because the ‘controller’ in Django is called
‘view’, while the ‘view’ is called ‘templates’, it did not really effect
much on their own function but it is better to rephrases as
Model–view–templates (MVT).

By the first touch of Django framework, reading documentation became
fairly important to me, but after reading the offical one it did not
actually gave me a full picture of what I supposed to get, so then I
decided to find some video tutorials to help me out for a deeper digging
into this framework, and those videos do helped me a lot since I was
able to see and follow their steps to quickly set up a example
application.

One of difficulties that I encountered was trying to distinguish the
Django and its API framework. The API framework was actually like widget
available in Django framework, and it have to be included manually
inside setting file to get it work. At the time I did not figure out
their relation between which made me fall behind with others’ progress
in our group. Not many videos are available online since just a few
people had worked on the API framework using Django, and even with all
that I still felt kind of blur overall. Getting back to official
documentation was what I took eventually, and drawing a diagram to
visualise what I learned was other approach to get head around with
it(as photos shown below).

The second difficulties was about understanding of data serialisation.
Because data in Django models would need to be translated to a
text-based format(xml, json, yaml), serialiser would be needed to do
this. I was confused quite a bit with which is serialise and which is
deserialise, so I went to the Django documentation having a look at
their code snippets which gave me more examples on when we should use
which. And it gave more understanding when I wrote them down into my
version of application.

*Evidence: my personal folder called ‘Botanical\_API’ on master branch*

The third one was about joining tables between different data models. It
became useful when a user searching a plant specs, we then were able to
gave them result along with their belonged collection. I looked at some
data model examples from Stack Overflow, wrote them down and tried to
find some similarities compare to our data models, and it do works. I
found joining table was a breakthrough point that would gave us those
plants specs along with its collections, then just following the example
to build a query set in a python function which would then gave all
desired plants information back.

*Evidence: a python file in ‘Botanical\_API’ called ‘Serializer.py’,
available in my personal folder on master branch*

Additionally, we have also worked on many to many relationship of
joining between tables, which I did not really figure that out with
other group member Matt. Same procedure I took from above but did not
work well. Liam was finally working that out using depth parameter which
was quite interesting direction to conquer this
problems.![](media/image1.jpeg){width="2.9581846019247595in"
height="4.211231408573928in"}![](media/image5.jpeg){width="2.966865704286964in"
height="4.189029965004375in"}

Reflection

Reflection could be covered in two aspects for this task:

Time Management

Problem-Solving ability

Group Corporation and Communication

I am deeply aware of I am not the person who can allocate time
efficiently, but this task do take my time management ability to a
higher level. One of the most good thing is each one of us have our own
focus during the task, and for me I have to be contributive otherwise if
anyone else works are depend on mine progress, it will be affected as
well. Therefore this really forced me to be efficient on assigned work.

When I come across with some technical problems, there were more than
one way to solve it. Have to say that I used to ask someone else which
seemed convenient but it did not really give me any experience on how to
resolve a similar problems by next time. The truth is I was overwhelmed
by that big amount of English documentations at beginning, and always
trying to find a shortcut to conquer, for example like StackOverflow
code snippets — copy and paste. It was in fact took me more time to
understand their logic and then fit it into my project. Changing of
strategy was needed at the time. What I did was getting back to the
documentation combined with watching some video tutorials. Soon writing
down what I have grasped of new knowledge which made me feeling more
comfortable than great amounts of reading.

Despite this, I could still be totally stuck by some really tricky
problems sometimes, group corporation and communication then becoming so
important at the time. I remembered that I was not doing this well in
software engineering class, but for this time I really tried to have a
proper communication with other group members. Communication establish
common ground, more importantly, they would able to know where you at of
the overall progress.

In conclusion, all these practices gave me more profound experiences on
how to be a better time manager, a better good contributor and a better
person.

Main Documentation Reference

Django framework:

[*https://www.djangoproject.com*](https://www.djangoproject.com);

[*https://tutorial.djangogirls.org/zh/django/*](https://tutorial.djangogirls.org/zh/django/);

[*https://www.youtube.com/watch?v=dM8Ncf5FNtM\#t=717.13633575*](https://www.youtube.com/watch?v=dM8Ncf5FNtM#t=717.13633575);

Django RESTful API framework:
[*http://www.django-rest-framework.org*](http://www.django-rest-framework.org);

Google CardBoard / Visual Scan Tools

Understanding and Difficulties

Cardboard Panorama Viewer

In this task what we were trying to delivery was a simple, fun, and
affordable way to let user experience virtual reality that provided a
360° immersive tour of some of our favourite New Zealand landscapes and
attractions.

Based on previous experience, we started this task by reading its
offical documentation. Since everyone of us was new to this technology,
we were vacillate between two approaches that provided in the
documentation: one was using Unity Engine, and the other one was to make
it to be a plain android application. We finally had a agree on this
with making it into a plain android app due to the time limit and
reduction of overall complexity.

There are more than one example provided in Google VR SDK and one of
them called ‘VrPanoViewer’ which gave me more general idea on how to
actually use it to display panorama photos. Just like other thirty party
library, google have offered us a pre-build panorama view just like a
TextView in Android studio by simply drag and drop to where we needed
it. Inside a class called ImageLoaderTask which inherited from AsyncTask
we feed our images as an array to assetManager, so then ‘goToNextScene’
method would able to retrieve next image by plus one to ‘panoIndex’
variable.

To understanding how it works basically took me not only reading its
example code but also looking up some finished project from others that
is available online, which is similar to the procedures of working out
model joining in Django. By narrowing down “unnecessary” code in the
example and adding my own comments on the side, I felt more confident to
handle more needs that intent to apply to this application.

*Evidence: a brief version of VrPanoViewer android App along with a
GoogleVRCodeUnderstanding documentation available in my personal folder
on master branch*

Apart from working with the base class, I was also assigned to work on
interface landscaping and doing a sensor checking on device. Inspired by
Apple Music bubble menu, I was thinking of implementing a similar one
which would be really great as then our users were able to select
certain images for viewing. Functionally worked same as a menu with
ticking boxes but will provided a more user-friendly interface in terms
of a better design philosophy. Implementing this seemed not that easy as
I imagined. The first problem was how to install a provided third party
library. After researches I knew that compile package dependency should
go into app’s gradle file not project one. The second was how to pass
user selected images to SimpleVrPanoramaActivity class. I found a
pre-made BubblePicker class provide a ‘getSelectedItems’ method, so I
simply used a for loop which looped through those items, got their
titles, put them into an array and then pass it to
SimpleVrPanoramaActivity class with ‘putExtra’ method leant from Android
Dev class. Finally that sensor checking method would show up an alert
dialogue if user’s device does not meet hardware requirements to get
into cardboard view mode.

*Evidence: VrPanoViewer in production branch. Documentation for this
launch screen is available in my personal folder on master
branch.*![](media/image9.png){width="1.9187784339457568in"
height="3.411161417322835in"}

![](media/image10.png){width="1.96462489063867in"
height="1.9537707786526683in"}

Visual Scanned Tool

We were approached by the Otago Polytechnic school of occupation therapy
with a request to build an all inclusive visual software suite, which
designed to aid people with impaired vision.

In this task I meanly focus on helping Andrew to display the camera
within a Cardboard View and be able to look around the environment in
real time. Since VR was designed to take people to a different world,
there were hardly any of this example available online. By a long time
of researching, there was a CameraPipeThrough app which would be able to
help us implement this. But basically it captured each frame from the
camera and use this to re-create it side by side. And because of this,
user might feeling a bit of dizzy due to camera frames overlay.

*Evidence: CardboardPassThrough App in my personal folder on master
branch*

The ideal outcome would be getting real time camera frames showing into
CardBoard View then blur it to suit tool’s needs. I finally get real
time blurring function working with a imported third party library. The
principle of the library is basically to grab each pixel of frames from
real camera, and then do a complex math algorithm for Red, Green, and
Blue, end by sending a recomputed colour back to camera view in order to
achieve a real time Gaussian Blur effect. But this still proved
challenging to the point where I was not able to replicate the processed
camera frames within a Cardboard layout.

*Evidence: CarmeraDemo App in my personal folder on master branch*

Reflection

Reflection could be covered in two aspects for this task:

Reading Documentation

Responsibility

Version Control on GitHub

I was not really count on reading offical documentation when I get a
touch with something new before to be honest. But for this project, by
now I really grasp this: “The more I read, the more I learnt” By now the
offical documentation is becoming to my first resource and it is not a
nightmare for me like even before because I have a better attitude
toward it.

Throughout project one paper, no matter which role you were acting, we
have to be responsible. I remembered I did software engineer last
semester and at the time I did not really handle that well, with low
participating and a bad communication skills with other group member, so
I felt like there was huge amount of pressure on we that always made
thinking what if I do not contribute enough this time. At the beginning
of very first task when I was still in a adapting time, others seems
getting faster and faster on their own hands, which made me anxious a
lot. Set a right pace on both physical progress of group project and
your psychological expectation of I have contributed is important and
hard. Also experiencing a scum master for two weeks gave me some new
thinking as well. I think it is very important to be able to receive
criticism, have others dismiss my ideas, and then have a proper
communication to find out where I could make progress by the next time.

In our group git policy simply offered us a coordinating and unifying
version control system. It is important for everyone one us pushing
their progress to let some else in the group to see others progress, and
this is what I should improve in the future by not just keep stalling
the stuff inside my own folder.
