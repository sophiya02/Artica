---
# BasketballUtils
---
## initialize()


Initialize the BasketballUtils Objects.

| param | type [= default] | description |
| ----- | ---------------- | ----------- |
---
## debug( string msg )


Logs a debug message if verbose mode is enabled.

| param   | type [= default] | description               |
| ------- | ---------------- | ------------------------- |
| **msg** | string           | The message to be logged. |
---
## getTeams()


Retrieves NBA teams data from the 'balldontlie.io' API and inserts it into a ServiceNow table.

| param  | type [= default] | description                             |
| ------ | ---------------- | --------------------------------------- |
| return | void             | This function does not return anything. |

 **Example** 
```//Returns list of teams this.getTeams();```

---
## getPlayerByID( string id )


Retrieves player data by ID from the 'balldontlie.io' API and inserts it into a ServiceNow table.

| param  | type [= default] | description                             |
| ------ | ---------------- | --------------------------------------- |
| **id** | string           | The ID of the player.                   |
| return | void             | This function does not return anything. |

 **Example** 
```//Returns Player for the given ID this.getPlayerById('abc123')```

---
## getAllPlayers()


Retrieves all the players from the 'balldontlie.io' API and inserts each player into a ServiceNow table.

| param  | type [= default] | description                             |
| ------ | ---------------- | --------------------------------------- |
| return | void             | This function does not return anything. |
---
## getGameByID( string id )


Retrieves games data by ID from the 'balldontlie.io' API and inserts it into a ServiceNow table.

| param  | type [= default] | description                             |
| ------ | ---------------- | --------------------------------------- |
| **id** | string           | The ID of the player.                   |
| return | void             | This function does not return anything. |
---
## getGamesByDate( Date dates )


Retrieves games data by date from the 'balldontlie.io' API and inserts it into a ServiceNow table.

| param     | type [= default] | description                             |
| --------- | ---------------- | --------------------------------------- |
| **dates** | Date             | The date of the game.                   |
| return    | void             | This function does not return anything. |
---
## getGamesByDateRange( Date start,Date end )


Retrieves games data by date range from the 'balldontlie.io' API and inserts them into a ServiceNow table.

| param     | type [= default] | description                             |
| --------- | ---------------- | --------------------------------------- |
| **start** | Date             | The start date of the Date Range.       |
| **end**   | Date             | The end date of the Date Range          |
| return    | void             | This function does not return anything. |
---
## getPlayerStatsByGame( string game )


Retrieves player stats of the game by gmae ID from the 'balldontlie.io' API and inserts it into a ServiceNow table.

| param    | type [= default] | description                             |
| -------- | ---------------- | --------------------------------------- |
| **game** | string           | The ID of the game.                     |
| return   | void             | This function does not return anything. |
---
## getGameIDsByDate( Date date )


Retrieves game ids by date from the 'balldontlie.io' API and return the ids of the games played that day.

| param    | type [= default] | description                                                                                                                   |
| -------- | ---------------- | ----------------------------------------------------------------------------------------------------------------------------- |
| **date** | Date             | The date of the game.                                                                                                         |
| return   | Array<string>    | This function returns ids of the game played on the particular date. // Returns Game on given data this.greeting("28/05/02"); |
---
## getGameIDsByDateRange( Date start,Date end )


Retrieves game ids by date range from the 'balldontlie.io' API and returns the game ids played in the date range.

| param     | type [= default] | description                                                      |
| --------- | ---------------- | ---------------------------------------------------------------- |
| **start** | Date             | The start date of the Date Range.                                |
| **end**   | Date             | The end date of the Date Range                                   |
| return    | Array<string>    | This function returns ids of the game played in the date ranges. |
---
## getYesterdayStatsForAllPlayers()


Retrieves player statistics for all players from the previous day's games and inserts them into a ServiceNow table.

| param  | type [= default] | description                             |
| ------ | ---------------- | --------------------------------------- |
| return | void             | This function does not return anything. |
---
## getAllPlayerStatsByDate( GlideDate date )


Retrieves player statistics for all players for a specified date and inserts them into a ServiceNow table.

| param    | type [= default] | description                                       |
| -------- | ---------------- | ------------------------------------------------- |
| **date** | GlideDate        | The date for which to retrieve player statistics. |
| return   | void             | This function does not return anything.           |
---
## getAllSeasonAvgForPlayer( string player )


Retrieves season averages for a player for each season starting from 1979 until the current year and inserts them into a ServiceNow table.

| param      | type [= default] | description                                                |
| ---------- | ---------------- | ---------------------------------------------------------- |
| **player** | string           | The ID of the player for whom to retrieve season averages. |
| return     | void             | This function does not return anything.                    |
---
## getSingleSeasonAvgForPlayer( number season,string player )


Retrieves season averages for a player for a specific season from the 'balldontlie.io' API and inserts them into a ServiceNow table.

| param      | type [= default] | description                                                |
| ---------- | ---------------- | ---------------------------------------------------------- |
| **season** | number           | The season for which to retrieve the averages.             |
| **player** | string           | The ID of the player for whom to retrieve season averages. |
| return     | void             | This function does not return anything.                    |
---
## getUpdatedSeasonAvgs()


Retrieves updated season averages for all players based on yesterday's game stats and inserts them into a ServiceNow table.

| param  | type [= default] | description                             |
| ------ | ---------------- | --------------------------------------- |
| return | void             | This function does not return anything. |
---
## getGamesPlayersStatsByRange( string start,string end )


Retrieves game statistics for players within a specified date range from the 'balldontlie.io' API and inserts them into a ServiceNow table.

| param     | type [= default] | description                                         |
| --------- | ---------------- | --------------------------------------------------- |
| **start** | string           | The start date of the range in 'YYYY-MM-DD' format. |
| **end**   | string           | The end date of the range in 'YYYY-MM-DD' format.   |
| return    | void             | This function does not return anything.             |
---
## getPlayerStatlinesByYear( string player,number year )


Retrieves player stat lines for a specific year from the 'balldontlie.io' API and inserts them into a ServiceNow table.

| param      | type [= default] | description                                           |
| ---------- | ---------------- | ----------------------------------------------------- |
| **player** | string           | The ID of the player for whom to retrieve stat lines. |
| **year**   | number           | The year for which to retrieve the stat lines.        |
| return     | void             | This function does not return anything.               |
---
## _sleepytime( number ms )


Pauses the execution for the specified duration in milliseconds.

| param  | type [= default] | description                             |
| ------ | ---------------- | --------------------------------------- |
| **ms** | number           | The duration to wait in milliseconds.   |
| return | void             | This function does not return anything. |
