Submits a score to an existing leaderboard. Song must have a leaderboard (see [create new leaderboard](create%20new%20leaderboard.md)) before you can submit scores for it. This will also overwrite and delete the user's previous score, regardless of if it was higher than before, so be sure to check the [my leaderboard position](my%20leaderboard%20position.md) endpoint before submitting.

POST `/leaderboards/song/:hash/submit`

Request Body:
- JSON in the form of a [leaderboard submission](../data%20types/leaderboard%20submission.md) object

Possible Responses:
- 200:
	- a [score submission response](../data%20types/score%20submission%20response.md)
- 401, 403, 404, or 520:
	- see [common error codes](../other/common%20error%20codes.md)