## 400
- You didn't send all required information in the request. (invalid parameters, incorrect request body, etc.)
## 401
- You didn't send an authorization header, or the one you sent was invalid (see [authenticating](authenticating.md)).
## 403
 - The meaning of this depends on the response content.
 - "You are blacklisted from making requests to this API."
	 - You were banned, probably for submitting cheated scores or abusing the API in some other way.
- "That song is blacklisted."
	- The song you were trying to make a leaderboard for is disallowed from having a leaderboard.
## 404
- The song you were trying to get a leaderboard for doesn't exist.
- In the case of a [my leaderboard position](../endpoints/my%20leaderboard%20position.md) request, you don't have a leaderboard position for that instrument/song combination.
## 520
 - Something unexpected happened when performing a database action. This *should* never happen, and if this is returned, something very bad has likely happened to the database.