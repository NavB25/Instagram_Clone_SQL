# SQL Instagram Clone

As an avid user of Instagram, it is difficult to truly grasp how complex of a database the app must have to manage well over 1 billion users worldwide! I was curious whether or not I could atleast replicate the fundemental design of Instagram with the use of SQL and with only 100 randomly generated users.

**Table Schema**

**users**
* id **(PK)**
* username
* created_at

**photos**
* id **(PK)**
* image_url
* user_id **(FK)**
* created_at

**comments**
* id **(PK)**
* comment_text
* photo_id **(FK)**
* user_id **(FK)**
* created_at

**likes**
* user_id **(PK,FK)**
* photo_id **(PK,FK)**
* created_at

**follows**
* follower_id **(PK,FK)**
* followee_id **(PK,FK)**
* created_at

**tags**
* id **(PK)**
* tag_name
* created_at

**photo_tags**
* photo_id **(PK,FK)**
* tag_id **(PK,FK)**
