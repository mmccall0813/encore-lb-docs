Gets a leaderboard for a song given a MIDI hash and instrument.

GET `/leaderboards/song/:hash`

Required parameters:
- instrument: what instrument-specific leaderboard you want to check from

Optional parameters:
- page: A number denoting which page you would like to view of the leaderboard.

Possible responses:
- code 200:
	- a [public leaderboard](../data%20types/public%20leaderboard.md) object
- code 404: 
	- see [common error codes](../other/common%20error%20codes.md)

Example response:
```json
{
    "scores": [
        {
            "submitter": {
                "display_name": "mmccall0813",
                "username": "macrottie",
                "discord_id": "100060265176924160"
            },
            "run": {
                "uuid": "006ba40a-67e6-44f1-8507-e46ae1c847d9",
                "score": 500,
                "note_count": 5,
                "notes_hit_good": 0,
                "notes_hit_perfect": 5,
                "misses": 0,
                "strikes": 0,
                "instrument": "plastic_guitar",
                "difficulty": 3
            },
            "leaderboard": {
                "position": 1
            }
        }
    ],
    "context": {
        "current_page": 1,
        "total_pages": 1,
        "total_scores": 1
    }
}
```