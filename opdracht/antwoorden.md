# Antwoorden Eindopdracht

1. Copy paste je gemaakte SQL query hieronder
   SELECT races.name,circuits.name AS races_circuit_laatste_jaar FROM races LEFT JOIN circuits ON races.circuitId =circuits.circuitId WHERE year= 2018

2. Copy paste je gemaakte SQL query hieronder
   SELECT races.name AS Race_name, drivers.surname,driver_standing.points FROM races LEFT JOIN driver_standing ON races.raceId = driver_standing.raceId LEFT JOIN drivers ON driver_standing.driverId = drivers.driverId WHERE races.year = 2017 AND driver_standing.points = 10

3. Copy paste je gemaakte SQL query hieronder
   SELECT drivers.forename,drivers.surname,pitstops.duration FROM races LEFT JOIN driver_standing ON races.raceId = driver_standing.raceId LEFT JOIN drivers ON driver_standing.driverId = drivers.driverId LEFT JOIN pitstops ON races.raceId = pitstops.raceId WHERE pitstops.duration <25;

4. Copy paste je gemaakte SQL query hieronder
   SELECT constructors.constructorRef AS constructors,races.name AS Grandprix FROM races LEFT JOIN constructor_standing ON races.raceId = constructor_standing.raceId LEFT JOIN constructors ON constructor_standing.constructorId = constructors.constructorId WHERE constructors.constructorRef="Mclaren" AND races.year=2017;

5. Copy paste je gemaakte SQL query hieronder
   SELECT circuits.name AS circuits, circuits.country AS land,races.name AS Grandprix FROM races LEFT JOIN circuits ON races.circuitId = circuits.circuitId LEFT JOIN driver_standing ON races.raceId = driver_standing.raceId LEFT JOIN drivers ON driver_standing.driverId = drivers.driverId WHERE drivers.surname LIKE "F%" AND year=1950;
