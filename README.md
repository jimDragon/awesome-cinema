# 🎥 Awesome Cinema
An awesome movie reservation system!

![dashboard](images/dashboard.png)
_Awesome Cinema - Dashboard_

## What is it?
Awesome Cinema is a **simple movie reservation** system based on LAMP (Linux, Apache, Mariadb, PHP) stack and it's part of my university assignment in Databases 1 course. It's also my first ever fullstack web application made entirely from scratch starting from the database ERD to frontend interface. Although this web app is far from being perfect it can provide a good starting point for a real Cinema reservation system.

![cinema_erd](images/cinema_erd.png)
_Awesome Cinema - ERD made with [draw.io](https://app.diagrams.net/)_ 

## Features
- Manage Customers
- Manage Sessions
- Manage Reservations
- Print tickets


## Assumptions
Because this is a univesity project, some assumptions regarding cinema organization were made in order to be a realistically achivable assignment. Some of them include:
- All the available sessions are considered active sessions.
- The seat configuration in a room doesn't follow any amphitheatrical principals.
- Each customer can reserve 5 tickets of a movie session and thus a maximum of 5 people should be considered in each reservation and later in the cinema room.
- By the time that a reservation is completed successfully, each customer in that reservation is free to choose and **any seat** in the movie room.

## Project setup
### Requirements
- Preferably a GNU/linux based operating system
- An Apache server which is run under `/srv/http/`
- Mariadb
- A web browser

### Installation
1. Clone the repository under `/srv/http/` path and make sure the folder name is `awesome_cinema`.
2. Log into mariadb and execute:
```
source database.sql
source insert_data.sql
```
3. Add your mariadb username and password to `config/database.php` file in the corresponding variables.
4. In your browser navigate to `localhost/awesome_cinema`
5. Enjoy :)

If the interface doesn't load the proper data you may have to change the permissions of the `/srv/http/`

## Screenshots
![customers](images/customers.png)
_Awesome Cinema - customer management_

![sessions](images/sessions.png)
_Awesome Cinema - session management_


![tickets](images/tickets.png)
_Awesome Cinema - ticket confirmation_

## License
[View here](https://github.com/jimDragon/awesome-cinema/blob/master/LICENSE)
