Instagram Clone Database
Welcome to the Instagram Clone Database! This database is designed to mimic the functionality of the popular social media platform Instagram. It contains tables for users, photos, likes, comments, hashtags, and more. This README provides an overview of the database structure, its tables, and basic usage instructions.

Table of Contents
Database Structure
Getting Started
Schema Overview
Queries and Usage
Contributing
License
Database Structure
The Instagram Clone Database is built using SQL and consists of several tables that work together to store user-generated content and interactions. Here's an overview of the main tables:

users: Stores user information such as usernames, emails, and profile data.
photos: Contains photo data, including URLs and creation timestamps.
likes: Records likes given by users to specific photos.
comments: Stores comments made by users on photos.
hashtags: Stores hashtags used in captions and comments, linked to relevant photos.
Getting Started
To set up the Instagram Clone Database on your local machine, follow these steps:

Clone this repository: git clone https://github.com/yourusername/instagram-clone-db.git
Create a new SQL database using your preferred database management system.
Import the SQL file instagram_clone_db.sql into your database.
Schema Overview
Here's a brief overview of the schema used in the database:

users

user_id (Primary Key)
username
email
...
photos

photo_id (Primary Key)
user_id (Foreign Key referencing users)
photo_url
created_at
...
likes

like_id (Primary Key)
user_id (Foreign Key referencing users)
photo_id (Foreign Key referencing photos)
created_at
...
comments

comment_id (Primary Key)
user_id (Foreign Key referencing users)
photo_id (Foreign Key referencing photos)
comment_text
created_at
...
hashtags

hashtag_id (Primary Key)
hashtag_name
...



Task:

1.How many times does the average user post?

2.Find the top 5 most used hashtags.

3.Find users who have liked every single photo on the site.

4.Retrieve a list of users along with their usernames and the rank of their account creation, ordered by the creation date in ascending order.

5.List the comments made on photos with their comment texts, photo URLs, and usernames of users who posted the comments. Include the comment count for each photo

6.For each tag, show the tag name and the number of photos associated with that tag. Rank the tags by the number of photos in descending order.

7.List the usernames of users who have posted photos along with the count of photos they have posted. Rank them by the number of photos in descending order.

8.Display the username of each user along with the creation date of their first posted photo and the creation date of their next posted photo.

9.For each comment, show the comment text, the username of the commenter, and the comment text of the previous comment made on the same photo.

10.Show the username of each user along with the number of photos they have posted and the number of photos posted by the user before them and after them, based on the creation date.
