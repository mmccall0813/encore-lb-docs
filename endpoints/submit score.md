Submits a score to an existing leaderboard. Song must have a leaderboard (see [[create new leaderboard]]) before you can submit scores for it. This will also overwrite and delete the user's previous score, regardless of if it was higher than before, so be sure to check the [[my leaderboard position]] endpoint before submitting.

POST `/leaderboards/song/:hash/submit`

Request Body:
- JSON in the form of a [[leaderboard submission]] object

Possible Responses:
- 200:
	- score submitted successfully
- 401, 403, 404, or 520:
	- see [[common error codes]]