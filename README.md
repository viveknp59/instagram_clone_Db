# Instagram Clone Database

Welcome to the Instagram Clone Database project! This repository contains the SQL database schema and sample data for an Instagram clone, allowing you to replicate some of the core functionality of the popular social media platform.

## Table of Contents

- [Database Structure](#database-structure)
- [Getting Started](#getting-started)
- [Schema Overview](#schema-overview)
- [Usage Examples](#usage-examples)
- [Contributing](#contributing)
- [License](#license)

## Database Structure

The Instagram Clone Database is designed using SQL and consists of multiple tables to store user information, photos, likes, comments, hashtags, and more. Below are the main tables in the schema:

- `users`: Stores user profiles, including usernames, emails, and other user-related data.
- `photos`: Contains photo records, including URLs, creation timestamps, and references to user IDs.
- `likes`: Records likes given by users to specific photos.
- `comments`: Stores user comments on photos, associated with both users and photos.
- `hashtags`: Manages hashtags used in photo captions and comments, linked to relevant photos.

## Getting Started

To set up and use the Instagram Clone Database on your local system, follow these steps:

1. Clone this repository to your local machine using `git clone https://github.com/yourusername/instagram-clone-db.git`.
2. Create a new SQL database using your preferred database management system (e.g., MySQL, PostgreSQL).
3. Import the SQL file `instagram_clone_db.sql` into your database to create the necessary tables and sample data.

## Schema Overview

Here's a brief overview of the database schema:

- `users`
  - `user_id` (Primary Key)
  - `username`
  - `email`
  - ...

- `photos`
  - `photo_id` (Primary Key)
  - `user_id` (Foreign Key referencing `users`)
  - `photo_url`
  - `created_at`
  - ...

- `likes`
  - `like_id` (Primary Key)
  - `user_id` (Foreign Key referencing `users`)
  - `photo_id` (Foreign Key referencing `photos`)
  - `created_at`
  - ...

- `comments`
  - `comment_id` (Primary Key)
  - `user_id` (Foreign Key referencing `users`)
  - `photo_id` (Foreign Key referencing `photos`)
  - `comment_text`
  - `created_at`
  - ...

- `hashtags`
  - `hashtag_id` (Primary Key)
  - `hashtag_name`
  - ...

## Usage Examples

You can perform various SQL queries to interact with the Instagram Clone Database, such as:

- Retrieve all photos posted by a specific user.
- Calculate the number of likes for a particular photo.
- Find the top 5 most used hashtags in the database.
- ...







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
