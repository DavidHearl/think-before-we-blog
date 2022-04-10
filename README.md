# Terminal Commands & Deployment

- pip3 install django gunicorn
- pip3 install dj_database_url psycopg2
- pip3 install dj3-cloudinary-storage
- pip3 freeze --local > requirements.txt
- django-admin startproject codestar .
- python3 manage.py startapp blog
- python3 manage.py migrate (after "blog" was added to installed apps in settings.py)
- python3 manage.py
- *** after deployment steps ***
- create new app on heroku
- recources > heroku postgres > settings > config vars > DATABASE_URL > copy
- create new file, env.py
- add DATABASE_URL
- add SECRET_KEY
- *** finsihed deployment steps ***
- python3 manage.py migrate
- *** to check go to heroku > resources > heroku postgres (data is then displayed) ***
- git add .
- git commit -m 
- git push

# Migrate changes

- python3 manage.py makemigrations
- python3 manage.py migrate

# Copy files to modify templates

- cp -r ../.pip-modules/lib/python3.8/site-packages/allauth/templates* ./templates

# Design Thinking

- View post list: As a Site User I can view a list of posts so that I can select one to read
- Open a post: As a Site User I can click on a post so that I can read the full text
- View likes: As a Site User / Admin I can view the number of likes on each post so that I can see which is the most popular or viral
- View comments: As a Site User / Admin I can view comments on an individual post so that I can read the conversation
- Account registration: As a Site User I can register an account so that I can comment and like
- Comment on a post: As a Site User I can leave comments on a post so that I can be involved in the conversation
- Like / Unlike: As a Site User I can like or unlike a post so that I can interact with the content
- Manage posts: As a Site Admin I can create, read, update and delete posts so that I can manage my blog content
- Create drafts: As a Site Admin I can create draft posts so that I can finish writing the content later
- Approve comments: As a Site Admin I can approve or disapprove comments so that I can filter out objectionable comments

# Database Models

- Move user stories into In progress
- Entity Relationship Diagram [Key, Name, Type]

