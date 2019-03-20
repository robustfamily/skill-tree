# skill-tree

SQL 

1 -----------------------------------------------------------------------------------------------------------------------
Adults only (SQL for Beginners #1)
https://www.codewars.com/kata/590a95eede09f87472000213

In your application, there is a section for adults only. You need to get a list of names and ages of users from the users table, who are 18 years old or older.
users table schema
name
age

my:
SELECT * FROM users
WHERE age BETWEEN 18 AND 999

best:
SELECT name, age FROM users WHERE age >= 18;

2 -----------------------------------------------------------------------------------------------------------------------
On the Canadian Border (SQL for Beginners #2)
https://www.codewars.com/kata/590ba881fe13cfdcc20001b4

You are a border guard sitting on the Canadian border. You were given a list of travelers who have arrived at your gate today. You know that American, Mexican, and Canadian citizens don't need visas, so they can just continue their trips. You don't need to check their passports for visas! You only need to check the passports of citizens of all other countries!
Select names, and countries of origin of all the travelers, excluding anyone from Canada, Mexico, or The US.
travelers table schema
name
country

my:
SELECT * FROM travelers WHERE country IN ('Italy', 'Spain', 'France', 'Egypt', 'Argentina', 'China')

best:
Select name,country from travelers where country not in ('Canada','Mexico','USA')


