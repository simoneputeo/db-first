| name                | type                                   | attributes               | index       |
| ------------------- | -------------------------------------- | ------------------------ | ----------- |
| id                  | INT                                    | NOT NULL, AUTO INCREMENT | PRIMARY KEY |
| brand               | VARCHAR(30)                            | NOT NULL                 | INDEX       |
| model               | VARCHAR(50)                            | NOT NULL                 | INDEX       |
| package             | VARCHAR(50)                            |                          | INDEX       |
| km                  | INT                                    | NOT NULL                 |             |
| state               | ENUM( "OK", "GOOD", "PERFECT", "KM0")  | NOT NULL                 |             |
| price               | INT                                    | NOT NULL                 |             |
| color               | VARCHAR(40)                            |                          |             |
| optionals           | TEXT                                   |                          |             |
| engine              | VARCHAR(30)                            |                          |             |
| engine_displacement | FLOAT (6,2)                            |                          |             |
| engine_power        | FLOAT (5,2)                            |                          |             |
| power_supply        | ENUM("DIESEL", "FUEL", "HYBRID", "EV") | NOT NULL                 |             |
| power_supply_extra  | ENUM("LPG", "METHANE", "HYDROGEN")     | NOT NULL                 |             |
| model_year          | YEAR                                   | NOT NULL                 | INDEX       |
| available           | ENUM("SHOWROOM", "GARAGE", "COMING")   | NOT NULL                 |             |
| nationality         | VARCHAR(40)                            | NOT NULL                 |             |
| license_plate       | VARCHAR(10)                            | NOT NULL                 | INDEX       |
| vin_code            | VARCHAR(40)                            | NOT NULL, UNIQUE         | INDEX       |
