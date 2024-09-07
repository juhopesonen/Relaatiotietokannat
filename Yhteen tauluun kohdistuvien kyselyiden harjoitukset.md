Yhteen tauluun kohdistuvien kyselyiden harjoitukset

tehtävä 1

select * from goal;

![image](https://github.com/user-attachments/assets/6b94d37c-7760-402b-9a52-8b4ca65359fd)

tehtävä 2

select name from airport where iso_country like "%FI%";

![image](https://github.com/user-attachments/assets/d842d4e6-bae6-41b9-9af8-c8ad11b5a7d3)

tehtävä 3

select name from airport where iso_country like "%FI%" order by name;

![image](https://github.com/user-attachments/assets/c91db2f1-c03c-4ec5-bf27-327147306bfa)

tehtävä 4

select name, type from airport where iso_country like "%FI%"order by type, name;

![image](https://github.com/user-attachments/assets/db09fb8e-5ddf-4a52-9c2a-d9ae3b22595f)

tehtävä 5

select name from country where name like "F%";

![image](https://github.com/user-attachments/assets/73f75d64-9c53-43b5-a77c-ce685760fa33)

tehtävä 6

select name from country where name like "%F%";

![image](https://github.com/user-attachments/assets/cf0ea78b-2689-4255-9d07-dd42e7eace52)

tehtävä 7

select location from game where screen_name = "Vesa";

![image](https://github.com/user-attachments/assets/1c1811ca-b3bf-4c65-a241-9bcbbcf29433)

tehtävä 8

select co2_consumed from game where screen_name = "Ilkka";

![image](https://github.com/user-attachments/assets/cde6ddfa-f6c7-4faa-8f72-15eecdbe8738)

tehtävä 9

select distinct co2_budget from game;

![image](https://github.com/user-attachments/assets/d8aaf463-2e59-4a0a-876a-a45a183f890e)

