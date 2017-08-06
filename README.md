
# SpartaScoop: # 

### Stay Connected to Campus ###

Contents
* [Project Description](#description)
* [Requirements](#requirements)
* [Web UI Requirement Principles - VOC, Personas, Job Shadowing](#req)
* [Web UI Design Principles – Storyboard, Wireframes](#principles)
* [Interfaces – RESTFul](#rest)
* [Server Side Design](#server)
* [High Level Architecture Design](#hlad)
* [Data Flow Diagram](#flow)
* [Sequence or Workflow](#sequence)
* [HTML5 Features Used](#html5)
* [Client Side Design](#clinet)
* [Testing (Stress test)](#test)
* [Cross Browser Compatibility](#cross)
* [Java Script Libraries – documentation](#js)
* [SEO](#seo)
* [Profiling](#profiling)
* [Website Analytics](#analytics)
* [Website Snapshots](#website)


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
<br>

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

## <a name="server"></a>Server Side Design ##
Following are the design patterns used in the project:
#### Adapter: ####
The Adapter pattern translates one interface (an object's properties and methods) to another. Adapters allows programming components to work together that otherwise wouldn't because of mismatched interfaces. The Adapter pattern is also referred to as the Wrapper Pattern.<br>
One scenario where Adapters are commonly used is when new components need to be integrated and work together with existing components in the application.<br>
Another scenario is refactoring in which parts of the program are rewritten with an improved interface, but the old code still expects the original interface.<br>
The portal uses the adapter pattern when it saves and retrieves images from the database in the following fashion:
![picture](/Documentation/img/designpattern.png)

## <a name="hlad"></a>High Level Architecture Design ##
![picture](/Documentation/img/hld.png)

## <a name="flow"></a>Data Flow Diagram ##
![picture](/Documentation/img/dataflow.png)

## <a name="sequence"></a>Sequence Diagram ##
![picture](/Documentation/img/sequence.png)

## <a name="html5"></a>HTML5 Features Used ##

Following HTML 5 features were used during the development of our website:
* &lt;article&gt;	Defines an article in a document
* &lt;aside&gt;		Defines content aside from the page content
* &lt;footer&gt;	Defines a footer for a document or section
* &lt;header&gt;	Defines a header for a document or section
* &lt;section&gt;	Defines a section in a document
* &lt;address&gt;	Defines contact information for the author/owner of a document
* &lt;progress&gt;	Represents the strength of a password
* &lt;figcaption&gt;	Defines a caption for a <figure> element
* &lt;wbr&gt;		Defines a possible line-break
* &lt;nav&gt;		Represents a section of the document intended for navigation.
* &lt;Email&gt;		Input type should be an email.
* &lt;search&gt;	Term to supply to a search engine. For example, the search bar atop a browser.
* &lt;canvas&gt;        HTML5 element <canvas> gives you an easy and powerful way to draw graphics using JavaScript. It can be used to draw graphs, make photo compositions or do simple (and not so simple) animations.
* &lt;figure&gt;        Represents a piece of self-contained flow content, typically referenced as a single unit from the main flow of the document.
New HTML5 attributes used:
* Autocomplete: The autocomplete attribute specifies whether or not an input field should have autocomplete enabled. Autocomplete allows the browser to predict the value. When a user starts to type in a field, the browser should display options to fill in the field, based on earlier typed values.
* Autofocus: The autofocus attribute is a Boolean attribute. When present, it specifies that an <input> element should automatically get focus when the page loads.


## <a name="client"></a>Client Side Design ##

Sparta Scoop is designed in a way which allows decoupling of the front end and the back-end to provision independent development of modules and features. <br>
Following are the pages through which the user can interact:
### Home page: ###
The index page is the page the user views on a successful login.
The index page has the following components:
* Feeds
Feeds on the index page allow a user to see the recent posts which have been made by him and other users of the website. The user can also see the posts which have been made by him separately on the right.
User can also create a new post on the index page.
* Links
Index page also contains links to all other pages of website, which allow him to navigate through the platform effortlessly.

### Jobs page: ###
The jobs page allows the user to view the available job posts which have been made by him or by other users. He can also post a new job on this page.
While posting new data, the user needs to provide every field which is required to create a job post. This allows a consistent post formats for all the jobs present on the platform. Also, it helps better reveal the job description and details.

### Accommodations page: ###
The accommodations page allows the user to view the available accommodations posts which have been made by him or by other users. He can also post a new accommodation on this page.
While posting new data, the user needs to provide every field which is required to create an accommodations post. This allows a consistent post formats for all the accommodations present on the platform. Also, it helps better reveal the accommodations description and details.
The page also features maps, to facilitate ease of finding the relevant accommodations for the user.

### Events page: ###
The events page allows the user to view the available events posts which have been made by him or by other users. He can also post a new event on this page.
While posting new data, the user needs to provide every field which is required to create an event post. This allows a consistent post formats for all the events present on the platform. Also, it helps better reveal the event description and details.

### Edit Profile: ###
This page allows user to update his details including his profile picture.

### Login/Signup: ###
Allows students to create new account or log into an existing account. Only people with valid SJSU email can register to the website.

### Admin dashboard: ###
Admin dashboard allows the website admin to monitor website related stats. This page contains various charts based on website usage, which gives better insights of how the platform is performing and what’s popular.


## <a name="test"></a>Testing (UI or Stress test) ##

![picture](/Documentation/img/testing/test1.png)

![picture](/Documentation/img/testing/test2.png)

![picture](/Documentation/img/testing/test3.png)


## <a name="cross"></a>Cross Browser Compatibility ##

Getting a page to look identical in different browsers is, sadly, far from simple.
This is because:
* Different browsers implement CSS styling in different ways
* Some browsers don’t support some css selectors
* Some browsers have bugs in their implementation of css

To provide consistent experience to users across all browsers, following steps were taken:
* Valid Code:
Used the W3C html validator and CSS validator while coding to check we haven’t made any silly mistakes.
* Used Firebug:
Firebug is a handy little plug-in for Firefox that lets you view the css applied to any particular element simply by highlighting it on screen. If you highlight code in the html Firebug will shade the item and display margins and padding.
* Used CSS @supports Rule
The CSS @supports allows you to wrap your CSS rules within the @supports query so that the rule will only be applied if it’s supported on a particular browser. If a rule isn’t supported, it’ll get skipped over as if the rule weren’t there, which can really come in handy for those properties you want to use but don’t want to look terrible if they happen to not be supported on a browser.
* Test Driven Development:
To be sure that the website provides consistent experience across all browsers, we tested all the features during development on the three most commonly used browsers-
	o	Mozilla Firefox
	o	Google Chrome
	o	Internet Explorer


## <a name="js"></a>Java Script Libraries – documentation ##

Following JavaScript libraries were used for the development of our website:
* Angular.js
AngularJS (commonly referred to as "Angular.js" or "AngularJS 1.X") is a JavaScript-based open-source front-end web application framework mainly maintained by Google and by a community of individuals and corporations to address many of the challenges encountered in developing single-page applications. It aims to simplify both the development and the testing of such applications by providing a framework for client-side model–view–controller (MVC) and model–view–viewmodel (MVVM) architectures, along with components commonly used in rich Internet applications. The front end of the platform uses Angular.js to provide dynamic content to users.
* Node.js & Express.js
Node.js is an open-source, cross-platform JavaScript run-time environment for executing JavaScript code server-side. Node.js enables JavaScript to be used for server-side scripting, and runs scripts server-side to produce dynamic web page content before the page is sent to the user's web browser. The back-end of the website is developed using Node and Express.
* Bootstrap.js
Bootstrap is a free and open-source front-end web framework for designing websites and web applications. It contains HTML- and CSS-based design templates for typography, forms, buttons, navigation and other interface components, as well as optional JavaScript extensions. Bootstrap helped us to provide consistent view of the website across all devices.
* Highcharts
Highcharts is a charting library written in pure JavaScript, offering an easy way of adding interactive charts to your web site or web application. Highcharts currently supports line, spline, area, areaspline, column, bar, pie, scatter, angular gauges, arearange, areasplinerange, columnrange, bubble, box plot, error bars, funnel, waterfall and polar chart types. Highcharts were used for monitoring the usage of our website in the admin dashboard page. 

## <a name="seo"></a>Search Engine Optimization Provisioning ##

Following methods have been incorporated in Sparta-Scoop for improving search engine optimization: 
1.	Provide a unique title for each page with important keywords near the beginning of the title. 
2.	Add a description meta tag to each page with a unique description for each page. 
3.	Name all the images with a related keyword. Use alt tags. Make images as small as possible. Use image optimizer. 
4.	Use .html links more preferably. 
5.	For all the image links, put keywords in the alt attribute text. 
6.	Keep the URL short and human readable. Avoid dynamic parameters whenever/wherever possible. 
7.	Use robots.txt to block the search engine from indexing few pages
8.	Use rel=” next” and rel=” prev” in the <head> tag to indicate the relationship between the URLs
9.	Declare language attribute in HTML page
10.	Use different URL for desktop and mobile devices. rel=” canonical” and rel=” alternate”.
11.	Remove all the scripts from the html pages.
12.	Add social meta tag to the web pages
13.	Increase page loading speed 
* Minify code by removing unnecessary white spaces
* Use CSS sprites to reduce server requests 
* Enable asynchronous downloading of external js files


## <a name="profiling"></a>Profiling ##

![picture](/Documentation/img/profiling/1.png)
![picture](/Documentation/img/profiling/2.png)
![picture](/Documentation/img/profiling/3.png)
![picture](/Documentation/img/profiling/4.png)
![picture](/Documentation/img/profiling/5.png)

## <a name="analytics"></a>Website Analytics ##

### Active Users ###
![picture](/Documentation/img/analytics/ActiveUserAnalytics.png)
### Client Analysis ###
![picture](/Documentation/img/analytics/ClientAnalysis.png)
### Device Analysis ###
![picture](/Documentation/img/analytics/DeviceAnalysis.png)
### Location Analysis ###
![picture](/Documentation/img/analytics/LocationAnalysis.png)
### Userflow Sankey Chart ###
![picture](/Documentation/img/analytics/Userflow-SankeyChart.png)
### User Session Analytics ###
![picture](/Documentation/img/analytics/UserSessionAnalytics.png)
### Visitor Analysis ###
![picture](/Documentation/img/analytics/VisitorAnalysis.png)

## <a name="website"></a>Website Snapshots##

### Admin monthly posts ###
![picture](/Documentation/img/website/Admin-monthlyPosts.png)
### Admin portal analysis charts ###
![picture](/Documentation/img/website/Admin-portal-analysischarts.png)
### Edit profile ###
![picture](/Documentation/img/website/Edit-profile.png)
### Localization available languages ###
![picture](/Documentation/img/website/Localization-Available_languages.png)
### Localization French ###
![picture](/Documentation/img/website/Localization-French.png)
### Localization-Hindi ###
![picture](/Documentation/img/website/Localization-Hindi.png)
### Login/signup page ###
![picture](/Documentation/img/website/Loginsignuppage.png)
### Timeline-accomodations ###
![picture](/Documentation/img/website/Timeline-accomodations.png)
### Timeline-events ###
![picture](/Documentation/img/website/Timeline-events.png)
### Timeline jobs ###
![picture](/Documentation/img/website/Timeline-jobs.png)
### Timeline-pagination ###
![picture](/Documentation/img/website/Timeline-pagination.png)
### Timeline-pagination 2###
![picture](/Documentation/img/website/Timeline-pagination2.png)
