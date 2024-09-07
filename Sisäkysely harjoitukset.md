tehtävä 1

select country.name 
from country, airport
where airport.iso_country = country.iso_country and
airport.name like "%Satsuma%";

![image](https://github.com/user-attachments/assets/5f509912-aa60-4c58-819c-547fd09896f4)

tehtävä 2

select airport.name 
from country, airport
where airport.iso_country = country.iso_country and
country.name like "%Monaco%";

![image](https://github.com/user-attachments/assets/64088d15-0d39-4c45-8d51-366762853299)

tehtävä 3

select screen_name 
from game, goal_reached, goal
where game_id = game.id and goal_id =goal.id and
goal.name = "CLOUDS";

![image](https://github.com/user-attachments/assets/36f6f3dd-b3b2-49c0-9e49-4d703899317b)

tehtävä 4

select country.name
from country
where iso_country not in
(select airport.iso_country
from airport);

![image](https://github.com/user-attachments/assets/04979980-d496-4c5d-b87b-6b5923e72439)

tehtävä 5

select name
from goal
where id not in
(select goal_id
from goal_reached where game_id not in
(select id 
from game where screen_name ="heini"));

![image](https://github.com/user-attachments/assets/a49bf843-9dd5-4612-9187-5c4437de7b8a)

