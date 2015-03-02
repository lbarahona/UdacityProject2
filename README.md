# UdacityProject2: Tournament Planner

This project is part of of Udacity's [Full-Stack Web Developer Nanodegree](https://www.udacity.com/course/nd004).

### Description

As described in the project description for the course, this project consists in a Python module that uses the PostgreSQL database to keep track of players and matches in a game tournament.

The game tournament uses the Swiss system for pairing up players in each round: players are not eliminated, and each player should be paired with another player with the same number of wins, or as close as possible.

### Running the project

The project can be excuted using Vagrant, you'll have to navigate to the `vagrant/` folder and execute the command `vagrant up`.
To run the test cases follow this steps:

- `vagrant ssh`(To login to the VM).
- `cd /vagrant/tournament`(To navigate to the project directory).
- Connect to PostgreSQL console by typing `psql`.
- In order to make sure you'll get a fresh database created, type `drop database tournament ;`.
- Create the tournament the database schema by typing `create database tournament ;`.
- To connect to the tournament database type `\c tournament`.
- Create the project table by typing  `\i tournament.sql`.
- Type `\q` to exit the PostgreSQL console.
- You are now ready to run the test cases for the tournament project, simply type `python tournament_test.py`.
