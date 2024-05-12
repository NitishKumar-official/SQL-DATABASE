
CONSTRAINTS:-
Rule for data in the table

NOT NULL     :-columns can not have a null value
UNIQUE       :-all value in column are different
DEFAULT      :-sets the default value of a column
CHECK        :-it can limit the values allowed in the column

1. NOT NULL

CREATE TABLE user(
id INT,
name VARCHAR(30) NOT NULL,
email VARCHAR(30) UNIQUE,
followers INT,
following INT
);

2.UNIQUE

CREATE TABLE user(
id INT,
name VARCHAR(30) NOT NULL,
email VARCHAR(30) UNIQUE,
followers INT,
following INT
);

3. DEFAULT

CREATE TABLE user(
id INT,
name VARCHAR(30) NOT NULL,
email VARCHAR(30) UNIQUE,
followers INT DEFAULT 0,
following INT
);

4. CHECK

CONSTRAINTS age_check CHECK(age>=10 AND city="Delhi")

CREATE TABLE user(
id INT,
age INT,
name VARCHAR(30) NOT NULL,
email VARCHAR(30) UNIQUE,
followers INT DEFAULT 0,
following INT,
CONSTRAINT age_check CHECK(age>=13)             age_check is optional
);
