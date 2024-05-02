---
title: BasketballUtils
sidebar_label: BasketballUtils
---

Creating a class called Basdketball Utills , to create reusable functions

0 | 1 | 2
--- | --- | ---
param | type [= default] | description

---
title: initialize
sidebar_label: initialize
---

Initialize the BasketballUtils Objects.

0 | 1 | 2
--- | --- | ---
param | type [= default] | description

---
title: debug
sidebar_label: debug
---

Logs a debug message if verbose mode is enabled.

0 | 1 | 2
--- | --- | ---
param | type [= default] | description
**msg** | string | The message to be logged.

---
title: getTeams
sidebar_label: getTeams
---

Retrieves NBA teams data from the 'balldontlie.io' API and inserts it into a ServiceNow table.

0 | 1 | 2
--- | --- | ---
param | type [= default] | description
return | void | This function does not return anything.

---
title: getPlayerByID
sidebar_label: getPlayerByID
---

Retrieves player data by ID from the 'balldontlie.io' API and inserts it into a ServiceNow table.

0 | 1 | 2
--- | --- | ---
param | type [= default] | description
**id** | string | The ID of the player.
return | void | This function does not return anything.

---
title: getAllPlayers
sidebar_label: getAllPlayers
---

Retrieves all the players from the 'balldontlie.io' API and inserts each player into a ServiceNow table.

0 | 1 | 2
--- | --- | ---
param | type [= default] | description
return | void | This function does not return anything.

---
title: getGameByID
sidebar_label: getGameByID
---

Retrieves games data by ID from the 'balldontlie.io' API and inserts it into a ServiceNow table.

0 | 1 | 2
--- | --- | ---
param | type [= default] | description
**id** | string | The ID of the player.
return | void | This function does not return anything.

---
title: getGamesByDate
sidebar_label: getGamesByDate
---

Retrieves games data by date from the 'balldontlie.io' API and inserts it into a ServiceNow table.

0 | 1 | 2
--- | --- | ---
param | type [= default] | description
**dates** | Date | The date of the game.
return | void | This function does not return anything.

---
title: getGamesByDateRange
sidebar_label: getGamesByDateRange
---

Retrieves games data by date range from the 'balldontlie.io' API and inserts them into a ServiceNow table.

0 | 1 | 2
--- | --- | ---
param | type [= default] | description
**start** | Date | The start date of the Date Range.
**end** | Date | The end date of the Date Range
return | void | This function does not return anything.

---
title: getPlayerStatsByGame
sidebar_label: getPlayerStatsByGame
---

Retrieves player stats of the game by gmae ID from the 'balldontlie.io' API and inserts it into a ServiceNow table.

0 | 1 | 2
--- | --- | ---
param | type [= default] | description
**game** | string | The ID of the game.
return | void | This function does not return anything.

---
title: getGameIDsByDate
sidebar_label: getGameIDsByDate
---

Retrieves game ids by date from the 'balldontlie.io' API and return the ids of the games played that day.

0 | 1 | 2
--- | --- | ---
param | type [= default] | description
**date** | Date | The date of the game.
return | Array<string> | This function returns ids of the game played on the particular date.

---
title: getGameIDsByDateRange
sidebar_label: getGameIDsByDateRange
---

Retrieves game ids by date range from the 'balldontlie.io' API and returns the game ids played in the date range.

0 | 1 | 2
--- | --- | ---
param | type [= default] | description
**start** | Date | The start date of the Date Range.
**end** | Date | The end date of the Date Range
return | Array<string> | This function returns ids of the game played in the date ranges.

---
title: getYesterdayStatsForAllPlayers
sidebar_label: getYesterdayStatsForAllPlayers
---

Retrieves player statistics for all players from the previous day's games and inserts them into a ServiceNow table.

0 | 1 | 2
--- | --- | ---
param | type [= default] | description
return | void | This function does not return anything.

---
title: getAllPlayerStatsByDate
sidebar_label: getAllPlayerStatsByDate
---

Retrieves player statistics for all players for a specified date and inserts them into a ServiceNow table.

0 | 1 | 2
--- | --- | ---
param | type [= default] | description
**date** | GlideDate | The date for which to retrieve player statistics.
return | void | This function does not return anything.

---
title: getAllSeasonAvgForPlayer
sidebar_label: getAllSeasonAvgForPlayer
---

Retrieves season averages for a player for each season starting from 1979 until the current year and inserts them into a ServiceNow table.

0 | 1 | 2
--- | --- | ---
param | type [= default] | description
**player** | string | The ID of the player for whom to retrieve season averages.
return | void | This function does not return anything.

---
title: getSingleSeasonAvgForPlayer
sidebar_label: getSingleSeasonAvgForPlayer
---

Retrieves season averages for a player for a specific season from the 'balldontlie.io' API and inserts them into a ServiceNow table.

0 | 1 | 2
--- | --- | ---
param | type [= default] | description
**season** | number | The season for which to retrieve the averages.
**player** | string | The ID of the player for whom to retrieve season averages.
return | void | This function does not return anything.

---
title: getUpdatedSeasonAvgs
sidebar_label: getUpdatedSeasonAvgs
---

Retrieves updated season averages for all players based on yesterday's game stats and inserts them into a ServiceNow table.

0 | 1 | 2
--- | --- | ---
param | type [= default] | description
return | void | This function does not return anything.

---
title: getGamesPlayersStatsByRange
sidebar_label: getGamesPlayersStatsByRange
---

Retrieves game statistics for players within a specified date range from the 'balldontlie.io' API and inserts them into a ServiceNow table.

0 | 1 | 2
--- | --- | ---
param | type [= default] | description
**start** | string | The start date of the range in 'YYYY-MM-DD' format.
**end** | string | The end date of the range in 'YYYY-MM-DD' format.
return | void | This function does not return anything.

---
title: getPlayerStatlinesByYear
sidebar_label: getPlayerStatlinesByYear
---

Retrieves player stat lines for a specific year from the 'balldontlie.io' API and inserts them into a ServiceNow table.

0 | 1 | 2
--- | --- | ---
param | type [= default] | description
**player** | string | The ID of the player for whom to retrieve stat lines.
**year** | number | The year for which to retrieve the stat lines.
return | void | This function does not return anything.

---
title: _sleepytime
sidebar_label: _sleepytime
---

Pauses the execution for the specified duration in milliseconds.

0 | 1 | 2
--- | --- | ---
param | type [= default] | description
**ms** | number | The duration to wait in milliseconds.
return | void | This function does not return anything.

