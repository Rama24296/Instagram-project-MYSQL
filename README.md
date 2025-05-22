# Instagram Database Project

This project is a simplified simulation of an Instagram-like platform using SQL. It includes schema definitions and data inserts for users, photos, comments, likes, follows, tags, and photo-tag associations.

## Database Schema

The project creates the following tables:

- *users*: Stores user accounts.
- *photos*: Stores photos uploaded by users.
- *comments*: Stores comments made by users on photos.
- *likes*: Tracks which user liked which photo.
- *follows*: Represents follower-followee relationships.
- *tags*: Stores tag names.
- *photo_tags*: Associates photos with tags.

## Setup Instructions

1. Ensure you have a MySQL-compatible database system installed.
2. Run the SQL script file Instagram Projectt.sql in your MySQL environment or using a tool like MySQL Workbench or phpMyAdmin.

   ```sql
   SOURCE Instagram\ Projectt.sql;

3. The script will:

Create the instagram_db database.

Set up the schema.

Populate the database with sample data.


Features :

Supports core social media functionality:

User creation

Posting photos

Commenting on photos

Liking photos

Following users

Tagging photos



Example Queries :

You can run queries like:

-- Get all photos posted by a specific user
SELECT * FROM photos WHERE user_id = 1;

-- Get all users who follow a specific user
SELECT follower_id FROM follows WHERE followee_id = 1;

-- Get all likes on a photo
SELECT * FROM likes WHERE photo_id = 10;
