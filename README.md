# logAnalysis

The third project for the [Udacity Full Stack Nanodegree
Program](https://classroom.udacity.com/nanodegrees/nd004/), featuring a quick 
[Vagrant](https://www.vagrantup.com/) machine serving a [fairly
large](https://d17h27t6h515a5.cloudfront.net/topher/2016/August/57b5f748_newsdata/newsdata.zip)
[PostgreSQL](https://www.postgresql.org/) database. 

We then connect to this Database via Python, and run some queries defined in
`newsdata.py`, giving us back:

```
What are the most popular three articles of all time?
	 1 - Candidate is jerk, alleges rival 	 -  338647 views
	 2 - Bears love berries, alleges bear 	 -  253801 views
	 3 - Bad things gone, say good people 	 -  170098 views
Who are the most popular article authors of all time?
	 1 - Ursula La Multa 		 -  507594 views
	 2 - Rudolf von Treppenwitz 		 -  423457 views
	 3 - Anonymous Contributor 		 -  170098 views
	 4 - Markoff Chaney 		 -  84557 views
On which days did more than 1% of requests lead to errors?
	 2016-07-17 - 2.26% errors
```

### Building

Launch Vagrant VM by running `vagrant up`, you can the log in with `vagrant
ssh`. 

Load the data, then use the command `psql -d news -f newsdata.sql` to connect a database and run queries!

Database includes:
* Ajthors Table: Information about the authors of articles.
* Articles Table: The articles themselves.
* Log Table : Entry for each time a user has accessed the site.
