Where-osan liitosehto harjoitukset

tehtävä 1

select country.name as "country name", airport.name as "airport name"
from airport, country
where airport.iso_country = country.iso_country and country.name = "Iceland";

![image](https://github.com/user-attachments/assets/20c2c7e1-ea79-4897-961a-e0f3322c209a)

tehtävä 2

select airport.name as "airport name"
from airport, country
where airport.iso_country = country.iso_country and country.name = "France" and airport.type = "large_airport";

![image](https://github.com/user-attachments/assets/aa4db374-f9f8-44d3-a886-0fb0475783e0)

tehtävä 3

select country.name as country_name, airport.name as airport_name
from airport, country
where airport.iso_country = country.iso_country and country.continent = "AN";

![image](https://github.com/user-attachments/assets/b86347d3-b47b-45d7-9357-add7ff484b86)

tehtävä 4

select elevation_ft
from airport, game
where location = ident and screen_name = "Heini";

![image](https://github.com/user-attachments/assets/2ae88eb2-b646-4519-b21c-98aba3970737)

tehtävä 5

select elevation_ft * 0.3048 as elevation_m
from airport, game
where location = ident and screen_name = "Heini";

![image](https://github.com/user-attachments/assets/8d579fcc-123f-4be0-b2c9-204376f0d753)

tehtävä 6

select name
from airport, game
where location = ident and screen_name = "Ilkka";

![image](https://github.com/user-attachments/assets/8ea24bfb-dfd0-43ea-ad9e-b788987d615d)

tehtävä 7

select country.name
from country, game, airport
where location = ident and 
airport.iso_country = country.iso_country and screen_name = "Ilkka";

![image](https://github.com/user-attachments/assets/40d54e1e-6d0e-4e85-a632-191f64721e08)


tehtävä 8
tehtävä 9
tehtävä 10
