# OPJJ-wanna-be

Functional requirements:
- View summoner stats and matches
- Update summoner stats and matches

Used Riot APIs
- SUMMONER-V4
- LEAGUE-V4
- MATCH-V5

Used libraries:
- sqlite3

Logic
Get summoner:
1 Check if summoner exists in DB	
2 If not
	get data from API
	update DB
	return data from DB
3 If does not get returned from API
	return "USER_DEOS_NOT_EXISTS"
4 If exists
5 Return data from DB

Update summoner (assuming he exists):
1 Update summoner stats
2 Get list of matchIds from API and update DB
	if there are no games, return "NO_MATCHES"
3 Get details about matches from matches list and send it to DB
4 Get summoner stats and matches from DB
	
