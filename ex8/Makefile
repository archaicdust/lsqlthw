
all: mydata.db
	sqlite3 -header -column -echo mydata.db < ex8.sql

ex9: mydata.db
	sqlite3 -header -column -echo mydata.db < ex9.sql

ex10: mydata.db
	sqlite3 -header -column -echo mydata.db < ex10.sql

ex11: mydata.db
	sqlite3 -header -column -echo mydata.db < ex11.sql


mydata.db: code.sql
	sqlite3 mydata.db < code.sql

code.sql:
	touch code.sql
	cat ../ex2/ex2.sql >> code.sql
	# cat ../ex3/ex?.sql >> code.sql
	cat ../ex3/ex3.sql >> code.sql
	cat ../ex3/ex4.sql >> code.sql
	cat ../ex3/ex5.sql >> code.sql
	cat ../ex3/ex6.sql >> code.sql
	cat ../ex3/ex7.sql >> code.sql

clean:
	rm -rf code.sql
	rm -rf mydata.db
