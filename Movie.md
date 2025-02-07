CREATE TABLE movies (
    id SERIAL PRIMARY KEY,
    title VARCHAR(100),
    genre VARCHAR(50),
    year INT
);

INSERT INTO movies (title, genre, year) VALUES ('Inception', 'Sci-Fi', 2010);
INSERT INTO movies (title, genre, year) VALUES ('The Dark Knight', 'Action', 2008);
INSERT INTO movies (title, genre, year) VALUES ('Interstellar', 'Sci-Fi', 2014);

SELECT * FROM movies WHERE genre='Sci-Fi';
