A leaderboard entry is sent by the [my leaderboard position](../endpoints/my%20leaderboard%20position.md) endpoint and an array of leaderboard entries along with some other data is sent by the [public song leaderboard](../endpoints/public%20song%20leaderboard.md) endpoint.

A leaderboard entry is structured like so:
```json
{
	"submitter": { // information about who submitted this score
		"display_name": String,
		"username": String,
		"discord_id": String
	},
	"run": { // some info about the run that was submitted
		"uuid": String, // a unique identifier for this specific run
		"score": Integer,
		"note_count": Integer,
		"notes_hit_good": Integer,
		"notes_hit_perfect": Integer,
		"misses": Integer,
		"strikes": Integer,
		"instrument": String,
		"difficulty": Integer, // 0 = easy, 3 = expert
	},
	"leaderboard": {
		"position": Integer
	}
}
```