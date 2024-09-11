A public leaderboard datatype is a list of [leaderboard entry](leaderboard%20entry.md) objects along with some data that tells you what page you're on, how many pages there are, and how many songs total there are.

A public leaderboard structured like so:
```json
{
	"scores": [...leaderboard entry objects],
	"context": {
		"current_page": Integer,
		"total_pages": Integer,
		"total_scores": Integer
	}
}
```