Spotify

Client ID 
=> 8a67c0c79e7b42ff9f5f0cd24efff740

Client Secret 
=> 508ca0e059c24c94a8751c4dc134fa17

http://localhost/callback/?code={CODE} 
=> AQDL48uTjtYqMTIYCtENNKmb-zz4Mlw_WrWoSlvXHMuBeXqC61AvPKB1fHFLUiZAfhrXhb4ctrLkMA5XFtv3NiLxQCyPws4pNat-02bI4a8U5eNrP3YhFd46BnbvlzN9RR9su6iv94lbSZkwz_ONjM3xAvjRIEPweeaLTY8rAQvbMcX_tKqX31uLjuw3NwwmFQBjOEH8vQS2-CFxgbndOJPmFxY_WuH74QvbfHTieeEL8ODgE4c

encode {SPOTIFY_CLIENT_ID}:{SPOTIFY_CLIENT_SECRET} 
=> OGE2N2MwYzc5ZTdiNDJmZjlmNWYwY2QyNGVmZmY3NDA6NTA4Y2EwZTA1OWMyNGM5NGE4NzUxYzRkYzEzNGZhMTc=

curl -X POST -H "Content-Type: application/x-www-form-urlencoded" -H "Authorization: Basic {BASE64}" -d "grant_type=authorization_code&redirect_uri=http://localhost/callback/&code={CODE}" https://accounts.spotify.com/api/token 
=> curl -X POST -H "Content-Type: application/x-www-form-urlencoded" -H "Authorization: Basic OGE2N2MwYzc5ZTdiNDJmZjlmNWYwY2QyNGVmZmY3NDA6NTA4Y2EwZTA1OWMyNGM5NGE4NzUxYzRkYzEzNGZhMTc=" -d "grant_type=authorization_code&redirect_uri=http://localhost/callback/&code=AQDL48uTjtYqMTIYCtENNKmb-zz4Mlw_WrWoSlvXHMuBeXqC61AvPKB1fHFLUiZAfhrXhb4ctrLkMA5XFtv3NiLxQCyPws4pNat-02bI4a8U5eNrP3YhFd46BnbvlzN9RR9su6iv94lbSZkwz_ONjM3xAvjRIEPweeaLTY8rAQvbMcX_tKqX31uLjuw3NwwmFQBjOEH8vQS2-CFxgbndOJPmFxY_WuH74QvbfHTieeEL8ODgE4c" https://accounts.spotify.com/api/token 