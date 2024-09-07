tehtävä 1

select country.name as "country name", airport.name as "airport name"
from airport, country
where airport.iso_country = country.iso_country and country.name = 'Finland' and
airport.scheduled_service = "yes";

![image](https://github.com/user-attachments/assets/c495a3f1-4c69-4060-b0fb-5c1a06758164)

tehtävä 2

select screen_name, airport.name
from game, airport
where location = ident;

![image](https://github.com/user-attachments/assets/c2a30bc3-febb-4225-8ab7-96a8e1fa3eb1)

tehtävä 3

select screen_name, country.name
from game, country, airport
where location = ident and airport.iso_country = country.iso_country;

![image](https://github.com/user-attachments/assets/8a032fb5-813c-4c0c-8520-10acc1ea9998)

tehtävä 4

select airport.name, screen_name
from airport left join game on ident = location where name like "%Hels%";

![image](https://github.com/user-attachments/assets/f01df168-7a8e-4b2a-81b6-cc619ed525f6)

tehtävä 5

select goal.name, screen_name
from goal
left join goal_reached on goal.id = goal_id left join game on game_id = game.id;

![image](https://github.com/user-attachments/assets/448e0719-7922-449b-8ee5-78682fb646fe)
