# Social-Network-API

![](https://img.shields.io/badge/Created%20by-Victor%20Cesar%20Lopez-blue?style=for-the-badge)  
![](https://img.shields.io/badge/Database-MongoDB-yellow?style=flat-square&logo=mongoDB)  ![](https://img.shields.io/badge/npm%20package-express-orange?style=flat-square&logo=npm) ![](https://img.shields.io/badge/npm%20package-mongoose-cyan?style=flat-square&logo=npm) ![](https://img.shields.io/badge/npm%20package-moment-%3CCOLOR%3E?style=flat-square&logo=npm)

## Table of Contents:  
[Description](#Description)  
[Walkthrough Videos](#Walkthrough-Videos)  
[Installation](#Installation)  
[Tests](#Tests)  
[License Details](#License-Details)    
[Questions](#Questions)  

## Description:
This is a set of API for a social network that uses a MongoDB database so that the website can handle large amounts of unstructured data, Express.js for routing, Mongoose ODM, and the moment package to format time stamps.


## Walkthrough Videos
[User Routes](x)  
[Friend Routes](x)  
[Thought Routes](x)  
[Reaction Routes](x)  

## Installation:
-Clone GitHub repository
-npm init
-Ensure that MongoDB and Express are installed on your computer.
-Invoke application using npm start.

## Tests:  

Testing restful API calls with Insomnia Core  

---
**`/api/users`**
* `GET` all users
* `POST` a new user:
    ```json
    // example data
    {
        "username": "lernantino",
        "email": "lernantino@gmail.com"
    }
    ```
---
**`/api/users/:userid`**
* `GET` a single user by its `_id` 
* `PUT` to update a user by its `_id`
* `DELETE` to remove user by its `_id`
---
**`/api/users/:userId/friends/:friendId`**
* `POST` to add a new friend to a user's friend list
* `DELETE` to remove a friend from a user's friend list
---
**`/api/thoughts`** 
* `GET` to get all thoughts
* `POST` to create a new thought
    ```json
    // example data
    {
    "thoughtText": "Here's a cool thought...",
    "username": "lernantino",
    "userId": "5edff358a0fcb779aa7b118b"
    }
    ```
---
**`/api/thoughts/:thoughtId`**
* `GET` to get a single thought by its `_id`
* `PUT` to update a thought by its `_id`
* `DELETE` to remove a thought by its `_id`
---

**`/api/thoughts/:thoughtId/reactions`**

* `POST` to create a reaction 
    ```json
    // example data
    {
    "reactionBody":"Hell Yeah!!",
    "username":"lernantino"
    }
    ```
---
**`/api/thoughts/:thoughtId/reactions/:reactionId`**
* `DELETE` remove a reaction by the `reactionId` 

## License Details: 
 This project is under no license.  

## Questions:
Please reach out to me at mflanigantwualumn@gmail.com