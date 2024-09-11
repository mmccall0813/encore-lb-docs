Gives the user their leaderboard position given a MIDI hash and an instrument.

GET `/leaderboards/song/:hash/me`

Parameters: 
- instrument: what instrument-specific leaderboard you want to check from

Possible responses:
- code 200:
	- a [[leaderboard entry]] object
- code 404, 401, 403, or 400:
	- see [[common error codes]]

Example response:
```json
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
```