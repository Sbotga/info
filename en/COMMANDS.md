- **English**
# Commands
Sbotga has a variety of commands! Documentation for all of them can be found below.

✅ means fully documented.
### Ranked Commands ✅
- `/ranked view [rank] [region]` - View a specific t100 user on ranked.
    - `[rank]`: The rank to view.
        - Optional if your PJSK account is linked for specified region.
    - `[region]`: What ranked region to view (eg. EN ranked user)
        - Optional, defaults to EN.
- `/ranked leaderboard [region]` - View the t100 ranked leaderboard.
    - `[region]`: What ranked region to view (eg. EN ranked leaderboard)
        - Optional, defaults to EN.
### Event Commands ✅
- `/event view [rank] [region] [character]` - View a specific t100 user on the current running event.
    - `[rank]`: The rank to view.
        - Optional if your PJSK account is linked for specified region.
    - `[region]`: What region to view (eg. EN current event)
        - Optional, defaults to EN.
    - `[character]`: The character chapter, if applicable (World Link)
        - Optional.
- `/event leaderboard [region] [character]` - View the t100 current running event leaderboard.
    - `[region]`: What ranked region to view (eg. EN ranked leaderboard)
        - Optional, defaults to EN.
    - `[character]`: The character chapter, if applicable (World Link)
        - Optional.
### Guess Commands
### Song Information Commands
### Other Information Commands
### User Progression Commands ✅
- `/b30 [region] [private] [filter]` - View the b30 plays (best 30 songs) of the account.
  - `[region]`: What linked account to view (eg. EN account b30).
      - Optional, defaults to EN.
  - `[private]`: Hide the account ID and name.
       - Optional, defaults to False.
  - `[filter]`: What filters (FC only or AP only) to display the b30 with.
      - Optional, defaults to all (FC and AP).
- `/progress [difficulty] [region] [private]` - View a difficulty's progress, looking at FCs, APs, and Clears.
  - `[difficulty]`: View progress of this difficulty.
      - Optional, defaults to Master.
  - `[region]`: What linked account to view (eg. EN account progress)
      - Optional, defaults to EN.
  - `[private]`: Whether to hide your PJSK name and ID, replacing it with your Discord name.
      - Optional, defaults to False.
- `/song progress [song] [region]` - View the progress of a specific PJSK song.
  - `[song]`: What song to view progress of.
      - Mandatory.
  - `[region]`: What linked account to view (eg. EN account song progress)
      - Optional, defaults to EN.
### User Data/Setting Commands
### Uncategorized Commands ✅
- `/help` - Sends you some features, as well as a link to this specific documentation page.
- `/info` - Sends you basic information on the bot, as well as a link to this Github.
- `/ping` - View Sbotga's latency.
