

all: ex12.db
	sqlite3 -echo ex12.db < ex12.sql

ex12.db:
	make -C ../ex8 -f ../ex8/Makefile clean
	make -C ../ex8 -f ../ex8/Makefile mydata.db
	cp ../ex8/mydata.db ex12.db
	make -C ../ex8 -f ../ex8/Makefile clean

clean:
	rm -rf ex12.db
