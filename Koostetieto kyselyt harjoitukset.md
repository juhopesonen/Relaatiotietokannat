tehtävä 1

select max(elevation_ft)
from airport;

![image](https://github.com/user-attachments/assets/98b3258c-ebc7-4dca-ac69-16e0b6c915e6)

tehtävä 2

select continent, count(*)
from country
group by continent;

![image](https://github.com/user-attachments/assets/f75b5f78-c135-4dc5-953a-aed0e5b0db95)

tehtävä 3

select screen_name, count(*)
from game, goal_reached
where id = game_id
group by screen_name;

![image](https://github.com/user-attachments/assets/ebd42e78-ba07-4743-acbc-a02f72410778)

tehtävä 4

select screen_name 
from game where co2_consumed in(select min(co2_consumed) from game);

![image](https://github.com/user-attachments/assets/69402beb-ac5b-4a26-8778-a2e43780a74d)

tehtävä 5

select country.name, count(*)
from airport, country
where airport.iso_country = country.iso_country
group by country.iso_country
order by count(*) desc
limit 50;

![image](https://github.com/user-attachments/assets/9ad54b74-6203-48a4-97b3-ea0d68b7d012)

tehtävä 6

select country.name
from airport, country
where airport.iso_country = country.iso_country
group by country.iso_country
having count(*) > 1000;

![image](https://github.com/user-attachments/assets/5eb22a56-0391-4726-87f1-0b77ca23cf11)

tehtävä 7

select name from airport
where elevation_ft in (select max(elevation_ft) from airport); 

![image](https://github.com/user-attachments/assets/cabb9b67-3c7f-488e-9845-d7b59c13eb6f)

tehtävä 8

select country.name
from country, airport
where country.iso_country = airport.iso_country
and elevation_ft in (select max(elevation_ft) from airport); 

![image](https://github.com/user-attachments/assets/54c527e5-af9e-467e-a2c8-7701a3dfc5f0)

tehtävä 9

select count(*)
from goal_reached, game
where game.id = game_id and screen_name = "Vesa";

![image](https://github.com/user-attachments/assets/3a83dc7d-8e7c-4c61-bc82-2d6e908954e8)

tehtävä 10

select name
from airport
where latitude_deg in(select min(latitude_deg) from airport);

![image](https://github.com/user-attachments/assets/e048a120-693b-4715-b6db-eb8e09750ad7)

