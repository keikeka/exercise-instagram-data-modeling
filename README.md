<p>
<h4 align="center">4Geeks Academy</h4>
<h2 align="center" style="margin: 0">Database model for Instagram</h2>
<h3 align="center" style="margin-top: 0">Keili Rosales</h3>
</p>

## Objective

The objective of this exercise is to simulate the Instagram data model that allows the user to log in, add username, name, email and password, as well as post an image with its description and also be able to comment on this and other posts. 

The project uses Python's SQLAlchemy library to generate the database and contains the following tables:

**User table**
Stores four main pieces of information: a username, which must be unique, a name (the person can add first and last name or just the first one), an email and a password. In addition to this, the User table establishes two relatable columns: one to track each user's Post and another to track the Followers.

**Post Table**
Simply stores a description of the post, an image address and the user.id. In addition, it establishes a relationship with the Comment table to track each comment the post receives.

**Comment table**
Simply stores a comment and the id of the commenting user and the commented post.

**Follower Table**
Stores foreign keys about the User, the follower represents someone who is following someone and following who is being followed.

The tables can be viewed in the src/models.py file.

## Application

1. Enter the environment `$ pipenv shell`
2. Install all dependencies `$ pipenv install`
3. Generate the diagram as many times as necessary `$ python src/models.py`
4. Open the diagram.png file to see the UML diagram.

## Technologies

- SQLAlchemy
- Flask
- Python

## Contributions

I'd love to get your appreciation or report on the code at https://github.com/keikeka/exercise-instagram-data-modeling

Thank you so much!