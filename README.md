# JokFlix — starter build

Responsive Arabic-first streaming discovery UI with TMDB metadata via Netlify Function.

## Setup
1. Deploy this repository to Netlify.
2. Add environment variable `TMDB_READ_ACCESS_TOKEN` (secret, Functions scope).
3. Redeploy. The browser never receives the TMDB token.
4. Browse homepage: trending, top rated, popular series, new movies and episodes.

## Important
This starter is a discovery/catalog interface. It does not provide unauthorized film/episode streams. Integrate only video sources you have permission to use. External player popup blocking cannot be guaranteed by an iframe wrapper; test each provider in a normal browser and remove providers that trigger abusive redirects.

## Netlify
`netlify.toml` is included. Function endpoint: `/.netlify/functions/tmdb?path=%2Ftrending%2Fall%2Fday`
