tehtävä 1

select max(elevation_ft)
from airport;

tehtävä 2

select continent, count(*)
from country
group by continent;

tehtävä 3

select screen_name, count(*)
from game, goal_reached
where id = game_id
group by screen_name;

tehtävä 4

select screen_name 
from game where co2_consumed in(select min(co2_consumed) from game);

tehtävä 5

select country.name, count(*)
from airport, country
where airport.iso_country = country.iso_country
group by country.iso_country
order by count(*) desc
limit 50;

tehtävä 6

select country.name
from airport, country
where airport.iso_country = country.iso_country
group by country.iso_country
having count(*) > 1000;

tehtävä 7

select name from airport
where elevation_ft in (select max(elevation_ft) from airport); 

tehtävä 8

select country.name
from country, airport
where country.iso_country = airport.iso_country
and elevation_ft in (select max(elevation_ft) from airport); 

tehtävä 9

select count(*)
from goal_reached, game
where game.id = game_id and screen_name = "Vesa";


tehtävä 10

select name
from airport
where latitude_deg in(select min(latitude_deg) from airport);
