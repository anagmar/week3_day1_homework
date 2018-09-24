Questions:

1. Return ALL the data in the 'movies' table.

SELECT * FROM movies

2. Return ONLY the name column from the 'people' table

SELECT name FROM people

3. Oops! Someone at CodeClan spelled Keith's name wrong! Change it to reflect the proper spelling.

UPDATE people
SET name = 'Keith Douglas'
WHERE id = 22;


4. Return ONLY your name from the 'people' table.

SELECT name FROM people
WHERE id = 1;


5. The cinema is showing 'Batman Begins', but Batman is DC, not Marvel! Delete the entry from the 'movies' table.

DELETE FROM movies
WHERE id = 9;

6. Create a new entry in the 'people' table with the name of one of the instructors.

INSERT INTO people(name)
VALUES('Craig Morton');


7. Pawel has decided to hijack our movie evening, Remove him from the table of people.

DELETE FROM people
WHERE id = 24;

8. The cinema has just heard that they will be holding an exclusive midnight showing of
'Avengers: Infinity War'!! Create a new entry in the 'movies' table to reflect this.

INSERT INTO movies(title, year, show_time)
VALUES ('Infinity Wars', 2018, '00:00');

10. The cinema would also like to make the Guardians movies a back to back feature. Find out the show time of "Guardians of the Galaxy" and set the show time of "Guardians of the Galaxy 2" to start two hours later.

UPDATE movies
SET show_time = 00:00
WHERE id = 16;



Extension
1. Delete multiple entries from your table in a single command.

DELETE FROM people
WHERE id BETWEEN 6 AND 8;

2. Select all the movies ordered by year in descending order.

SELECT * FROM movies
ORDER BY year DESC;
