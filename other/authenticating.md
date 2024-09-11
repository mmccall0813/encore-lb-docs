To access an authorized endpoint, you need to include an authorization header with your request. The header should contain your API key encoded into base64 with "`Bearer `"  at the beginning.

Example of a valid auth header (assuming the API key exists on the server):
```
authorization: Bearer eW91dHViZS5jb20vd2F0Y2g/dj1kUXc0dzlXZ1hjUQ==
```

### Obtaining an API key
An API key can be acquired via running the slash command "`/apikey`" in any server containing the leaderboard bot. An API key can also be obtained by going to the authentication URL in the website config and allowing the encore leaderboards application to access basic user data. (`config.json > discord > oauth2_url`)