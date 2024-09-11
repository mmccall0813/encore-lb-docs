The create new leaderboard registers a song's metadata into the database. This has to be done before you can submit a score through the [[submit score]] endpoint.

POST `/leaderboards/song/:hash/create`

Request Body:
- JSON in the form of a [[song submission]] object

Possible responses:
- 200: 
	- song leaderboard created, and you can now submit scores to it.
- 409: 
	- song already has a leaderboard associated with it.
- 401, 403, 404, or 520: 
	- see [[common error codes]]