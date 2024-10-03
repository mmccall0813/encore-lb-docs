A score submission response is sent when you send a valid POST request to the [submit score](../endpoints/submit%20score.md) endpoint.

It is structured like so:
```json
{
	"leaderboard": {
		"pos": Integer, // where the user stands on the leaderboard
		"diff": Integer // how much their leaderboard position changed
	}
}
```