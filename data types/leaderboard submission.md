A leaderboard submission is the info that you need to send with a [submit score](../endpoints/submit%20score.md) endpoint call.

A leaderboard submission is structured like so:
```json
{
	"song_hash": String,
	"score": Integer,
	"note_count": Integer,
	"notes_hit_perfect": Integer,
	"notes_hit_good": Integer,
	"misses": Integer,
	"strikes": Integer,
	"instrument": String,
	"difficulty": Integer
}
```