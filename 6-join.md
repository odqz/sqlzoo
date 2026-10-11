# Answers for join
https://sqlzoo.net/wiki/The_JOIN_WC2026

1. `SELECT game,team,player,gtime FROM goal  WHERE player = 'Leandro Trossard'`
2. `SELECT id, teamname, coach FROM team WHERE id = 'BEL'`
3. `SELECT player, gtime, teamname FROM team JOIN goal ON team.id = goal.team WHERE gtime < 8`
4. `SELECT player, teamname, coach FROM goal JOIN team ON goal.team = team.id WHERE coach LIKE 'Sébastien%'`
5. `SELECT player, game, city FROM goal JOIN game ON goal.game = game.id WHERE player = 'Harry Edward Kane'`
6. `SELECT player, team FROM goal JOIN game ON goal.game = game.id WHERE city = 'Vancouver'`
7. `SELECT player, teamname FROM goal JOIN team ON goal.team = team.id JOIN game ON goal.game = game.id WHERE city = 'Vancouver'`
8. `SELECT city, teamname FROM game JOIN team ON game.team1 = team.id OR game.team2 = team.id WHERE played = '2026-07-01'`
9. `SELECT teamname, player FROM team JOIN game ON team.id = game.team1 OR team.id = game.team2 JOIN goal ON game.id = goal.game WHERE played = '2026-07-02' AND goal.team = team.id`
10. `SELECT played, player, pos FROM game JOIN goal ON game.id = goal.game JOIN player ON goal.player = player.playername WHERE city = 'Mexico City'`
11. ``
12. ``