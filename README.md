# SJSU Scoop # 

### Stay Connected to Campus ###

Contents
* [Project Description](#description)
* [Requirements](#requirements)
<!--
* [Web UI Requirement Principles - VOC, Personas, Job Shadowing](#req)
* [Web UI Design Principles – Storyboard, Wireframes](#principles)
* [Interfaces – RESTFul](#rest)
* [Server Side Design](#server)
* [High Level Architecture Design](#hlad)
* [Data Flow Diagram](#flow)
* [Sequence or Workflow](#sequence)
* [HTML5 Features Used](#html5)
* [Client Side Design](#client)
* [Testing (Stress test)](#test)
* [Cross Browser Compatibility](#cross)
* [Java Script Libraries – documentation](#js)
* [SEO](#seo)
* [Profiling](#profiling)
* [Website Analytics](#analytics)
* [Website Snapshots](#website)
-->

## <a name="description"></a>Project Description ##
Sparta-Scoop is an attempt to ease the life of college students. It aims to address all those problems which are common for a college goer, and which can be solved through a network of students and alumni.<br>
The idea is unique and has infinite potential because each year thousands of students join higher studies in the USA, and face common issues and concerns, such as deciding which courses to enroll for, which professors to choose, finding accommodations, jobs and internships. Such problems are amplified for international students, who are new to USA and are not familiar with the college life here.<br>
Even though some websites have tried to address some of these issues, they haven’t been completely successful. On the other hand, SpartaScoop tackles all issues on a single platform, which is designed in a way that it can be extended and customized based on the needs of a specific college or university.The developers of this solution are all international students, and have been through all the scenarios where community help and student cooperation are of ultimate help. Thus, we have aimed to incorporate all those features, which can be of help to a student.<br>
The first version of our platform has been designed specifically for San Jose State University students, and we have limited ourselves to three important issues:
*	Jobs and internships
*	Accommodations
*	On campus events <br>

Based on the popularity of the initial release, we plan to incorporate several more features like:
*	Course and professor reviews
*	Buy and sell items
*	Online tutoring<br>

We also plan to release our platform for other universities, by customizing it to the needs and requirements of the specific university.<br>
To prevent external influence, the website is only accessible to people who hold a valid email id of sjsu.edu domain.

## <a name="requirements"></a>Requirements ##

*	Students with valid email address can sign up and use the platform.
*	Registered users can make new posts and can view existing posts.
*	All users can view the jobs posted on job page.
*	All users can view the accommodations listed on accommodations page.
*	All users can view the events listed on the events page.
*	Every registered user can post accommodations, jobs and events.
*	Posted accommodations are visible on google maps.
*	Job posts need to have all the necessary fields as listed on the job posts.
*	Events posts need to have all the necessary fields as listed on the portal.
*	Admin can delete user profiles.
*	Admin can view usage statistics, top 5 users and other parameters when logged in through admin-login.
*	Admin can view the current website sessions and can monitor traffic, traffic locations.
*	User can update his/her profile.
*	Every user must have a unique identification email.
*	User can search for a specific job, update, delete job posts.
*	User can search for a specific accommodation, update, delete accommodation posts.
*	User can search for a specific event, update, delete event posts.

## <a name="req"></a>Web UI Requirement Principles - VOC, Personas, Job Shadowing ##

### Voice of the Customer(VOC) ###
Voice of the customer (VOC) is a term used in business and Information Technology (through ITIL, for example) to describe the in-depth process of capturing customer's expectations, preferences and aversions. <br>
Specifically, the Voice of the Customer is a market research technique that produces a detailed set of customer wants and needs, organized into a hierarchical structure, and then prioritized in terms of relative importance and satisfaction with current alternatives. <br>
Voice of the Customer studies typically consist of both qualitative and quantitative research steps. They are generally conducted at the start of any new product, process, or service design initiative to better understand the customer's wants and needs. <br>
To capture the voice of our customers(students), we created a survey and took responses from students all over SJSU campus. The responses helped us evaluate the needs of SJSU students, and through the results of this survey, we could zero-in on our features for our first release.<br>

Here are the results of our survey:

![picture](/Documentation/img/survey1.png)
<br>
![picture](/Documentation/img/survey2.png)

### Personas ###

A persona is a fictional character that communicates the primary characteristics of a group of users, identified and selected as a key target through use of segmentation data, across the company in a usable and effective manner.
Sparta-Scoop is based on the following personas:
Students:
The primary user of the platform. This user uses the platform for gaining information posted on it by other students. The website must be able to provide relevant information every time a student logs in, he should also be able to share any information which can prove useful to other website users.
The student should not be presented with irrelevant information, neither should he be troubled with incorrect or fraudulent posts.
Alumni: 
The students should be able to mark themselves as alumni or current students, based on whether they have graduated or not. Once graduated, the student should still be able to access the portal through an identification unique to the alumni.

### Job Shadowing ###
Job shadowing and contextual interviews are two techniques used to find out what people do, where they need help, and how your product can help them. To do that, we accompanied people while they do their jobs and talked to them about their jobs.
Following methods were used for job shadowing:
* Interaction with various students on campus.
* Interaction with various student communities.
* Discussing and analyzing problems faced by us as students at SJSU
* Creating a survey out of those responses.
* Discussing common problems and ideas with students and staff while on campus.
* Analyzing the results of our survey.

## <a name="principles"></a>Web UI Design Principles – Storyboard, Wireframes ##

### Wireframes ###

A website wireframe, also known as a page schematic or screen blueprint, is a visual guide that represents the skeletal framework of a website. Wireframes are created for arranging elements to best accomplish a particular purpose. <br>

Following wireframes were used for designing our website:

![picture](/Documentation/img/wireframe/login.png)
<br>
![picture](/Documentation/img/wireframe/homepage.png)
<br>
![picture](/Documentation/img/wireframe/jobspage.png)
<br>
![picture](/Documentation/img/wireframe/eventspage.png)
<br>
![picture](/Documentation/img/wireframe/accomodaionpage.png)
<br>
![picture](/Documentation/img/wireframe/admindash.png)
<br>


## <a name="rest"></a>Interfaces – RESTful ##
Representational state transfer (REST) or RESTful Web services are one way of providing interoperability between computer systems on the Internet. REST-compliant Web services allow requesting systems to access and manipulate textual representations of Web resources using a uniform and predefined set of stateless operations.<br>
Sparta-Scoop has been developed in a completely RESTful way to provide extensibility and reusability, so that it can be modified for other universities as well. <br>
The backend has been developed through Node.js and Express.js. The file server.js contains all endpoints which are provided by the server.<br>
