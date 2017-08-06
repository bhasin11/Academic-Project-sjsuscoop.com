
# SpartaScoop: # 

### Stay Connected to Campus ###

Contents
* [Project Description](https://github.com/bhasin11/Academic-Project-spartascoop.com/blob/addDocuments/README.md/#abc)
* [Requirements](https://github.com/bhasin11/Algorithms-in-JavaScript/blob/master/src/queue.js)
* [Web UI Requirement Principles - VOC, Personas, Job Shadowing](https://github.com/bhasin11/Algorithms-in-JavaScript/blob/master/src/circularQueue.js)
* [Web UI Design Principles – Storyboard, Wireframes](https://github.com/bhasin11/Algorithms-in-JavaScript/blob/master/src/linkedList.js)
* [Interfaces – RESTFul & Server Side Design](https://github.com/bhasin11/Algorithms-in-JavaScript/blob/master/src/doublyLinkedList.js)
* [High Level Architecture Design](https://github.com/bhasin11/Algorithms-in-JavaScript/blob/master/src/doublyLinkedList.js)
* [Data Flow Diagram](https://github.com/bhasin11/Algorithms-in-JavaScript/blob/master/src/doublyLinkedList.js)
* [Sequence or Workflow](https://github.com/bhasin11/Algorithms-in-JavaScript/blob/master/src/doublyLinkedList.js)
* [HTML5 Features Used](https://github.com/bhasin11/Algorithms-in-JavaScript/blob/master/src/doublyLinkedList.js)
* [Client Side Design](https://github.com/bhasin11/Algorithms-in-JavaScript/blob/master/src/doublyLinkedList.js)
* [Testing (UI or Stress test)](https://github.com/bhasin11/Algorithms-in-JavaScript/blob/master/src/doublyLinkedList.js)|
* [Automation (Selenium)](https://github.com/bhasin11/Algorithms-in-JavaScript/blob/master/src/doublyLinkedList.js)
* [Cross Browser Compatibility](https://github.com/bhasin11/Algorithms-in-JavaScript/blob/master/src/doublyLinkedList.js)
* [Java Script Libraries – documentation](https://github.com/bhasin11/Algorithms-in-JavaScript/blob/master/src/doublyLinkedList.js)
* [Design Patterns Used](https://github.com/bhasin11/Algorithms-in-JavaScript/blob/master/src/doublyLinkedList.js)
* [Pagination](https://github.com/bhasin11/Algorithms-in-JavaScript/blob/master/src/doublyLinkedList.js)
* [Localization](https://github.com/bhasin11/Algorithms-in-JavaScript/blob/master/src/doublyLinkedList.js)
* [SEO](https://github.com/bhasin11/Algorithms-in-JavaScript/blob/master/src/doublyLinkedList.js)
* [Profiling](https://github.com/bhasin11/Algorithms-in-JavaScript/blob/master/src/doublyLinkedList.js)


## Project Description ##
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


## Requirements ##
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

## Web UI Requirement Principles - VOC, Personas, Job Shadowing ##

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

## Web UI Design Principles – Storyboard, Wireframes ##

### Wireframes ###

A website wireframe, also known as a page schematic or screen blueprint, is a visual guide that represents the skeletal framework of a website. Wireframes are created for arranging elements to best accomplish a particular purpose. <br>

Following wireframes were used for designing our website:

![picture](/Documentation/img/wireframe/login)
<br>
![picture](/Documentation/img/wireframe/homepage)
<br>
![picture](/Documentation/img/wireframe/jobspage)
<br>
![picture](/Documentation/img/wireframe/eventspage)
<br>
![picture](/Documentation/img/wireframe/accomodaionpage)
<br>
![picture](/Documentation/img/wireframe/admindash)
<br>


## Interfaces – RESTful & Server Side Design ##
Representational state transfer (REST) or RESTful Web services are one way of providing interoperability between computer systems on the Internet. REST-compliant Web services allow requesting systems to access and manipulate textual representations of Web resources using a uniform and predefined set of stateless operations.<br>
Sparta-Scoop has been developed in a completely RESTful way to provide extensibility and reusability, so that it can be modified for other universities as well. <br>
The backend has been developed through Node.js and Express.js. The file server.js contains all endpoints which are provided by the server.<br>
### Endpoints ###
Following are the various endpoints which are used for interacting with the backend and share data:

    URI {hostname}/v1/users
    HTTP Method HTTP GET
    Body {
    "_id": "5913c1eefbcd7c32c53cebcb",
    "username": "Amit Pandey",
    "user_emailid": "abcdefgh@sjsu.edu",
    "user_password": "1234",
    "__v": 0,
    "user_profilepicture_url": "data:image/png;base64,iVBORw0KGgoAAAANSUh",
    "user_major": "Software Engineering",
    "user_degree": "MS"
    }
    Return – Success HTTP 200 Ok
    Return - Failure HTTP 500 - { "message" : "Unable to fetch users"}
<br>

    URI {hostname}/v1/users
    HTTP Method HTTP POST
    Body {
    "username": "Amit Pandey",
    "user_emailid": "abcdefgh@sjsu.edu",
    "user_password": "1234",
    "user_profilepicture_url": "data:image/png;base64,iVBORw0KGgoAAAANSUh",
    "user_major": "Software Engineering",
    "user_degree": "MS"
    }
    Return – Success HTTP 200 Ok
    Return - Failure HTTP 500 - { "message" : "Unable to register user"}
    HTTP 404 - { "message" : "Email already registerd"}
<br>

    URI {hostname}/v1/users/:emailid
    HTTP Method HTTP GET
    Body {
    "username": "Amit Pandey",
    "user_emailid": "abcdefgh@sjsu.edu",
    "user_password": "1234",
    "user_profilepicture_url": "data:image/png;base64,iVBORw0KGgoAAAANSUh",
    "user_major": "Software Engineering",
    "user_degree": "MS"
    }
    Return – Success HTTP 200 Ok
    Return - Failure HTTP 500 - {"message": "Failed to find user"}
    HTTP 404 - { "message" : "User not found"}
    Action Delete User
<br>

    URI {hostname}/v1/users/:user_emailid
    HTTP Method HTTP DELETE
    Body none
    Return – Success HTTP 200 Ok - {"message" : "User deleted"}
    Return - Failure HTTP 500 - {"message" : "Unable to delete user"}
    Action Update User
<br>

    URI {hostname}/v1/users/:user_emailid
    HTTP Method HTTP PUT
    Body {
    "username": "Amit Pandey",
    "user_emailid": "abcdefgh@sjsu.edu",
    "user_password": "1234",
    "user_profilepicture_url": "data:image/png;base64,iVBORw0KGgoAAAANSUh",
    "user_major": "Software Engineering",
    "user_degree": "MS" }
    Return – Success HTTP 200 Ok - {"message" : "User deleted"}
    Return - Failure HTTP 500 - {"message" : "Unable to delete user"}
    Action User Login
<br>
<br>

    URI {hostname}/v1/users/login
    HTTP Method HTTP POST
    Body {
    "email":"gaurav.misra@sjsu.edu",
    "password":"keval"
    }
    Return – Success HTTP 200 Ok - {"message":"Login successful"}
    Return - Failure HTTP 404 - { "message" : "User not found"}
    Action Check email validity
<br>

    URI {hostname}/v1/users/:user_emailid/checkunique
    HTTP Method HTTP GET
    Body none
    Return – Success HTTP 200 Ok - { "message" : "Email is unique"}
    Return - Failure HTTP 404 - { "message" : "Email already exists"}
    Action Get User jobs
    URI {hostname}/v1/users/:userid/jobs
    HTTP
    Method
    HTTP GET
    Body [{
    "_id": "5911564ad44a58382c8ea507",
    "type": "ISA",
    "title": "Grading assistant for Prof Ranjan",
    "description": "Apply only if you have taken the coures",
    "location": "180",
    "email": "ranjan@sjsu.edu",
    "url": "www.ranjan.com",
    "dateposted": "09.07.2017",
    "departement": "SE",
    "payrate": 10,
    "postedby": "590f5eb7ec96bf2b5cdd3421",
    "postedbydetails": {
    "_id": "590f5eb7ec96bf2b5cdd3421",
    "username": "kaushikshingne",
    "user_emailid": "kaushik.shingne@sjsu.edu",
    "user_password": "pqr",
    "user_profilepicture_url":
    "https://avatars3.githubusercontent.com/u/4065884?v=3&u=a0ac43ec7cabf27ed83139f0674e0c9d46e12ea3&
    s=400",
    "user_degree": "masters",
    "user_major": "IE",
    "__v": 0
    },
    "__v": 0
    }]
    Return –
    Success
    HTTP 200 Ok
    Return -
    Failure
    HTTP 404 - { "message" : "Unable to fetch jobs"}
    Action Get user events
<br>

    URI {hostname}/v1/users/:userid/events
    HTTP
    Method
    HTTP GET
    Body [{
    "_id": "5911633a6d41382684bd9120",
    "title": "Welcome party",
    "description": "Festival of indian students",
    "location": "CE 180",
    "website": "www.iso.com",
    "entryfees": 10,
    "__v": 0,
    "postedby": "590f5eb7ec96bf2b5cdd3421",
    "postedbydetails": {
    "_id": "590f5eb7ec96bf2b5cdd3421",
    "username": "kaushikshingne",
    "user_emailid": "kaushik.shingne@sjsu.edu",
    "user_password": "pqr",
    "user_profilepicture_url":
    "https://avatars3.githubusercontent.com/u/4065884?v=3&u=a0ac43ec7cabf27ed83139f0674e0c9d46e12ea3&
    s=400",
    "user_degree": "masters",
    "user_major": "IE",
    "__v": 0
    },
    "free_stuffs": [
    "yes"
    ]
    }]
    Return –
    Success
    HTTP 200 Ok
    Return -
    Failure
    HTTP 404 - { "message" : "Unable to fetch events"}
    Action Get user accommodations
<br>

    URI {hostname} /v1/users/:userid/accomodations
    HTTP Method HTTP GET
    Body [{
    "_id": "59113c72eed996106020a26c",
    "type": "Temporary",
    "vacancies": 5,
    "preference": "girls",
    "startdate": "08-20-2017",
    "facilities": "2NHK, Swimming Pool, jacuzi",
    "apartment": "101 E San Fernando",
    "address": "San Jose",
    "lattitude": "72.089890",
    "longitude": "23.989879",
    "contact": "650 469 2736",
    "rent": 200,
    "postedby": "590f5eb7ec96bf2b5cdd3421",
    "postedbydetails": {
    "_id": "590f5eb7ec96bf2b5cdd3421",
    "username": "kaushikshingne",
    "user_emailid": "kaushik.shingne@sjsu.edu",
    "user_password": "pqr",
    "user_profilepicture_url":
    "https://avatars3.githubusercontent.com/u/4065884?v=3&u=a0ac43ec7cabf27ed83139f0674e0c9d46
    e12ea3&s=400",
    "user_degree": "masters",
    "user_major": "IE",
    "__v": 0
    },
    "__v": 0}]
    Return – Success HTTP 200 Ok
    Return - Failure HTTP 404 - { "message" : "Unable to fetch accomodations"}
    Action Check email validity
<br>

    URI {hostname}/v1/users/:user_emailid/checkunique
    HTTP Method HTTP GET
    Body none
    Return – Success HTTP 200 Ok - { "message" : "Email is unique"}
    Return - Failure HTTP 404 - { "message" : "Email already exists"}
    Action Get jobs
<br>

    URI {hostname}/v1/jobs
    HTTP Method HTTP GET
    Body [{
    "_id": "591408ab2965d23d46f990a0",
    "type": "TA",
    "title": "k",
    "description": "k",
    "location": "k",
    "email": "k",
    "url": "k",
    "dateposted": "k",
    "payrate": "k",
    "postedby": "590f5eb7ec96bf2b5cdd3421",
    "postedbydetails": {
    "_id": "590f5eb7ec96bf2b5cdd3421",
    "username": null,
    "user_emailid": null,
    "user_password": "xxxxxxxxxx",
    "user_profilepicture_url": null,
    "user_degree": "masters",
    "user_major": "IE"
    },
    "__v": 0
    }]
    Return – Success HTTP 200 Ok
    Return - Failure HTTP 500 - { "message" : "Unable to fetch jobs"}
    Action Get job
<br>

    URI {hostname}/v1/jobs/ :jobid
    HTTP Method HTTP GET
    Body {
    "_id": "591408ab2965d23d46f990a0",
    "type": "TA",
    "title": "k",
    "description": "k",
    "location": "k",
    "email": "k",
    "url": "k",
    "dateposted": "k",
    "payrate": "k",
    "postedby": "590f5eb7ec96bf2b5cdd3421",
    "postedbydetails": {
    "_id": "590f5eb7ec96bf2b5cdd3421",
    "username": null,
    "user_emailid": null,
    "user_password": "xxxxxxxxxx",
    "user_profilepicture_url": null,
    "user_degree": "masters",
    "user_major": "IE"
    },
    "__v": 0
    }
    Return – Success HTTP 200 Ok
    Return - Failure HTTP 500 - { "message" : "Unable to fetch job"}
    Action Save job
<br>

    URI {hostname}/v1/jobs
    HTTP Method HTTP POST
    Body {
    "_id": "591408ab2965d23d46f990a0",
    "type": "TA",
    "title": "k",
    "description": "k",
    "location": "k",
    "email": "k",
    "url": "k",
    "dateposted": "k",
    "payrate": "k",
    "postedby": "590f5eb7ec96bf2b5cdd3421",
    "postedbydetails": {
    "_id": "590f5eb7ec96bf2b5cdd3421",
    "username": null,
    "user_emailid": null,
    "user_password": "xxxxxxxxxx",
    "user_profilepicture_url": null,
    "user_degree": "masters",
    "user_major": "IE"
    },
    "__v": 0
    }
    Return – Success HTTP 200 Ok
    Return - Failure HTTP 500 - { "message" : "Unable to save job"}
    Action Delete job
<br>

    URI {hostname}/v1/jobs/:jobid
    HTTP Method HTTP Delete
    Body none
    Return – Success HTTP 200 Ok - { "status" : "Job deleted" }
    Return - Failure HTTP 500 - { "message" : "Unable to delete job"}
    Action Update job
<br>

    URI {hostname}/v1/jobs/:jobid
    HTTP Method HTTP PUT
    Body {
    "_id": "591408ab2965d23d46f990a0",
    "type": "TA",
    "title": "k",
    "description": "k",
    "location": "k",
    "email": "k",
    "url": "k",
    "dateposted": "k",
    "payrate": "k",
    "postedby": "590f5eb7ec96bf2b5cdd3421",
    "postedbydetails": {
    "_id": "590f5eb7ec96bf2b5cdd3421",
    "username": null,
    "user_emailid": null,
    "user_password": "xxxxxxxxxx",
    "user_profilepicture_url": null,
    "user_degree": "masters",
    "user_major": "IE"},
    "__v": 0}
    Return – Success HTTP 200 Ok
    Return - Failure HTTP 500 - { "message" : "Failed to update job"}
    Action Get Events
<br>

    URI {hostname}/v1/events
    HTTP Method HTTP GET
    Body [{
    "_id": "591167b02691333e4c576af3",
    "title": "SJSU Spartans VS CSULA Mavericks",
    "description": "Basketball game",
    "location": "SJSU",
    "website": "www.sjsu.com",
    "entryfees": 30,
    "__v": 0,
    "postedby": "590f5eb7ec96bf2b5cdd3421",
    "postedbydetails": {
    "_id": "590f5eb7ec96bf2b5cdd3421",
    "username": "kaushikshingne",
    "user_emailid": "kaushik.shingne@sjsu.edu",
    "user_password": "pqr",
    "user_profilepicture_url": "https://avatars3.githubusercontent.com/u/4065884?v=3&u=
    a0ac43ec7cabf27ed83139f0674e0c9d46e12ea3&s=400",
    "user_degree": "masters",
    "user_major": "IE",
    "__v": 0
    },
    "free_stuffs": [
    "yes"
    ]
    }]
    Return – Success HTTP 200 Ok
    Return - Failure HTTP 500 - { "message" : "Unable to fetch events"}
    Action Get Event
<br>

    URI {hostname}/v1/events/:eventId
    HTTP Method HTTP GET
    Body none
    Return – Success HTTP 200 Ok – Event json object
    Return - Failure HTTP 500 - { "message" : "Unable to fetch event”}
    Action Create Event
<br>

    URI {hostname}/v1/events
    HTTP
    Method
    HTTP POST
    Body [{
    "_id": "591167b02691333e4c576af3",
    "title": "SJSU Spartans VS CSULA Mavericks",
    "description": "Basketball game",
    "location": "SJSU",
    "website": "www.sjsu.com",
    "entryfees": 30,
    "__v": 0,
    "postedby": "590f5eb7ec96bf2b5cdd3421",
    "postedbydetails": {
    "_id": "590f5eb7ec96bf2b5cdd3421",
    "username": "kaushikshingne",
    "user_emailid": "kaushik.shingne@sjsu.edu",
    "user_password": "pqr",
    "user_profilepicture_url": "https://avatars3.githubusercontent.com/u/4065884?v=
    3&u=a0ac43ec7cabf27ed83139f0674e0c9d46e12ea3&s=400",
    "user_degree": "masters",
    "user_major": "IE",
    "__v": 0
    },
    "free_stuffs": [
    "yes"
    ]
    }
    Return –
    Success
    HTTP 200 Ok
    Return -
    Failure
    HTTP 500 - { "message" : "Unable to fetch event”}
    Action Create Event
<br>

    URI {hostname}/v1/events/ :eventid
    HTTP Method HTTP PUT
    Body Event json object
    Return – Success HTTP 200 Ok
    Return - Failure HTTP 500 - { "message" : "Unable to update event”}
    Action DELETE Event
<br>

    URI {hostname}/v1/events/ :eventid
    HTTP Method HTTP DELETE
    Body none
    Return – Success HTTP 200 Ok
    Return - Failure HTTP 500 - { "message" : "Unable to delete event”}
    Action Get Accomodations
<br>

    URI {hostname}/v1/accommodations
    HTTP Method HTTP GET
    Body []
    Return – Success H{
    "_id": "59113ce1eed996106020a26d",
    "type": "Permanent",
    "vacancies": 1,
    "preference": "boys",
    "startdate": "07-08-2017",
    "facilities": "2NHK, nothing",
    "apartment": "101 E San Fernando",
    "address": "Fremont",
    "lattitude": "72.089890",
    "longitude": "23.989879",
    "contact": "650 469 2736",
    "rent": 400,
    "postedby": "590f5eb7ec96bf2b5cdd3421",
    "postedbydetails": {
    "_id": "590f5eb7ec96bf2b5cdd3421",
    "username": "kaushikshingne",
    "user_emailid": "kaushik.shingne@sjsu.edu",
    "user_password": "pqr",
    "user_profilepicture_url": "https://avatars3.githubusercontent.com/u/4065884?v=3&u=
    a0ac43ec7cabf27ed83139f0674e0c9d46e12ea3&s=400",
    "user_degree": "masters",
    "user_major": "IE",
    "__v": 0
    },
    "__v": 0
    }TTP 200 Ok
    Return - Failure HTTP 500 - { "message" : "Unable to fetch accomodations”}
    Action Get Accomodation
<br>

    URI {hostname}/v1/accommodations/:accid
    HTTP Method HTTP GET
    Body {
    "_id": "59113ce1eed996106020a26d",
    "type": "Permanent",
    "vacancies": 1,
    "preference": "boys",
    "startdate": "07-08-2017",
    "facilities": "2NHK, nothing",
    "apartment": "101 E San Fernando",
    "address": "Fremont",
    "lattitude": "72.089890",
    "longitude": "23.989879",
    "contact": "650 469 2736",
    "rent": 400,
    "postedby": "590f5eb7ec96bf2b5cdd3421",
    "postedbydetails": {
    "_id": "590f5eb7ec96bf2b5cdd3421",
    "username": "kaushikshingne",
    "user_emailid": "kaushik.shingne@sjsu.edu",
    "user_password": "pqr",
    "user_profilepicture_url": "https://avatars3.githubusercontent.com/u/4065884?v=
    3&u=a0ac43ec7cabf27ed83139f0674e0c9d46e12ea3&s=400",
    "user_degree": "masters",
    "user_major": "IE",
    "__v": 0
    },
    "__v": 0
    }
    Return – Success HTTP 200 Ok
    Return - Failure HTTP 500 - { "message" : "Unable to fetch accomodation”}
    Action Save Accomodation
<br>

    URI {hostname}/v1/accommodations
    HTTP Method HTTP POST
    Body {
    "_id": "59113ce1eed996106020a26d",
    "type": "Permanent",
    "vacancies": 1,
    "preference": "boys",
    "startdate": "07-08-2017",
    "facilities": "2NHK, nothing",
    "apartment": "101 E San Fernando",
    "address": "Fremont",
    "lattitude": "72.089890",
    "longitude": "23.989879",
    "contact": "650 469 2736",
    "rent": 400,
    "postedby": "590f5eb7ec96bf2b5cdd3421",
    "postedbydetails": {
    "_id": "590f5eb7ec96bf2b5cdd3421",
    "username": "kaushikshingne",
    "user_emailid": "kaushik.shingne@sjsu.edu",
    "user_password": "pqr",
    "user_profilepicture_url": "https://avatars3.githubusercontent.com/u/4065884?v=3
    &u=a0ac43ec7cabf27ed83139f0674e0c9d46e12ea3&s=400",
    "user_degree": "masters",
    "user_major": "IE",
    "__v": 0
    },
    "__v": 0
    }
    Return – Success HTTP 200 Ok
    Return - Failure HTTP 500 - { "message" : "Unable to save accomodation”}
    Action Update Accomodation
<br>

    URI {hostname}/v1/accommodations/:accid
    HTTP Method HTTP PUT
    Body {
    "_id": "59113ce1eed996106020a26d",
    "type": "Permanent",
    "vacancies": 1,
    "preference": "boys",
    "startdate": "07-08-2017",
    "facilities": "2NHK, nothing",
    "apartment": "101 E San Fernando",
    "address": "Fremont",
    "lattitude": "72.089890",
    "longitude": "23.989879",
    "contact": "650 469 2736",
    "rent": 400,
    "postedby": "590f5eb7ec96bf2b5cdd3421",
    "postedbydetails": {
    "_id": "590f5eb7ec96bf2b5cdd3421",
    "username": "kaushikshingne",
    "user_emailid": "kaushik.shingne@sjsu.edu",
    "user_password": "pqr",
    "user_profilepicture_url": "https://avatars3.githubusercontent.com/u/4065884?v=
    3&u=a0ac43ec7cabf27ed83139f0674e0c9d46e12ea3&s=400",
    "user_degree": "masters",
    "user_major": "IE",
    "__v": 0
    },
    "__v": 0
    }
    Return – Success HTTP 200 Ok
    Return - Failure HTTP 500 - { "message" : "Unable to update accomodation”}
    Action Delete Accomodation
<br>

    URI {hostname}/v1/accommodations/:accid
    HTTP Method HTTP PUT
    Body none
    Return – Success HTTP 200 Ok
    Return - Failure HTTP 500 - { "message" : "Unable to update accomodation”}
    Action Get post counts
<br>

    URI {hostname}/v1/analytics/postcounts
    HTTP Method HTTP GET
    Body None
    Return – Success HTTP 200 Ok - {
    "events": 10,
    "jobs": 9,
    "accomodations": 3
    }
    Return - Failure
    Action Get major counts
<br>

    URI {hostname}/v1/analytics/majorcounts
    HTTP Method HTTP GET
    Body None
    Return – Success HTTP 200 Ok - {
    "IE": 1,
    "CS": 1,
    "SE": 2,
    "EE": 0,
    "CE": 0
    }
    Return - Failure
    Action Get price range for accommodations counts
<br>

    URI {hostname}/v1/analytics/accomodationprices
    HTTP Method HTTP GET
    Body None
    Return – Success HTTP 200 Ok -{
    "low": 2,
    "mid": 1,
    "high": 0
    }
    Return - Failure
    Action Get job rates
<br>

    URI {hostname}/v1/analytics/accomodationprices
    HTTP Method HTTP GET
    Body None
    Return – Success HTTP 200 Ok -{
    "low": 1,
    "mid": 2,
    "high": 1
    }
    Return - Failure
    Action Get events counts
<br>

    URI {hostname}/v1/analytics/accomodationprices
    HTTP Method HTTP GET
    Body None
    Return – Success HTTP 200 Ok -{
    "low": 4,
    "mid": 4,
    "high": 2
    }
    Return - Failure
    Action Get events counts
<br>

    URI {hostname}/v1/analytics/accomodationprices
    HTTP Method HTTP GET
    Body None
    Return – Success HTTP 200 Ok -{
    "low": 4,
    "mid": 4,
    "high": 2
    }
    Return - Failure
    Action Get feed
<br>

    URI {hostname}/v1/feed
    HTTP Method HTTP GET
    Body None
    Return – Success HTTP 200 Ok
    Return - Failure HTTP 500

### Server Side Design ###
Following are the design patterns used in the project:
#### Adapter: ####
The Adapter pattern translates one interface (an object's properties and methods) to another. Adapters allows programming components to work together that otherwise wouldn't because of mismatched interfaces. The Adapter pattern is also referred to as the Wrapper Pattern.<br>
One scenario where Adapters are commonly used is when new components need to be integrated and work together with existing components in the application.<br>
Another scenario is refactoring in which parts of the program are rewritten with an improved interface, but the old code still expects the original interface.<br>
The portal uses the adapter pattern when it saves and retrieves images from the database in the following fashion:
![picture](/Documentation/img/designpattern.png)



