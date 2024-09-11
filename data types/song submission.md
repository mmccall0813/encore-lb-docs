A song submission is an object that establishes the metadata a song has in the database, it consists of basic information about the song, along with how difficult each part is.

A song submission is structured like so:
```json
{
    song_hash: String,
    title: String,
    artist: String,
    album: String,
    charters: String,
    source: String,
    diff_drums: Integer,
    diff_bass: Integer,
    diff_guitar: Integer,
    diff_vocals: Integer,
    diff_plastic_drums: Integer,
    diff_plastic_bass: Integer,
    diff_plastic_guitar: Integer,
    song_length: Integer
}
```