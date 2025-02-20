- **한국어**
# 명령어
Sbotga는 다양한 명령을 수행할 수 있습니다! 이 곳에서 모든 명령어에 대한 설명을 찾을 수 있습니다.

`<argument>` - 필수 입력란입니다.

`[argument]` - 선택 입력란입니다.

> [!노트]  
> 매개변수 `song`의 자동완성에는 곡의 로마자 표기와 약어가 포함되지 않습니다. 다만, 둘 다 인식이 가능합니다.
> 매개변수 `song` 과 `character`는 "fuzzy match" (가까운 문자로 번역하기) 기능을 시도합니다. (따라서 오타가 나도 작동합니다)
### 랭크 매치 명령어
- `/ranked view [rank] [region]` - View a specific t100 user on ranked.
    - `[rank]`: The rank to view.
        - Optional if your PJSK account is linked for specified region.
    - `[region]`: What ranked region to view (eg. EN ranked user)
        - Optional, defaults to your default region (EN if not set).
- `/ranked leaderboard [region]` - View the t100 ranked leaderboard.
    - `[region]`: What ranked region to view (eg. EN ranked leaderboard)
        - Optional, defaults to your default region (EN if not set).
### Event Commands
- `/event view [rank] [region] [character]` - View a specific t100 user on the current running event.
    - `[rank]`: The rank to view.
        - Optional if your PJSK account is linked for specified region.
    - `[region]`: What region to view (eg. EN current event)
        - Optional, defaults to your default region (EN if not set).
    - `[character]`: The character chapter, if applicable (World Link)
        - Optional.
- `/event leaderboard [region] [character]` - View the t100 current running event leaderboard.
    - `[region]`: What event region to view (eg. EN event leaderboard)
        - Optional, defaults to your default region (EN if not set).
    - `[character]`: The character chapter, if applicable (World Link)
        - Optional.
- `/event schedule [region]` - View the upcoming event schedule.
    - `[region]`: What event region to view (eg. EN event schedule)
        - Optional, defaults to your default region (EN if not set).
- `/event border [region]` - View the current event borders (highlights).
    - `[region]`: What event region to view (eg. EN event border)
        - Optional, defaults to your default region (EN if not set).
### Guess Commands
- `/guess hint` - Get a hint for the current ongoing guess.
- `/guess end` - End the current ongoing guess.
- `/guess stats <guess_type> [lb_rank] [user]` - View the guess stats of a specified user.
    - `<guess_type>`: What type of guess.
    - `[lb_rank]`: What leaderboard rank the user is. Incompatible with `[user]`.
        - Optional, defaults to [user] OR yourself.
    - `[user]`: What user to check leaderboard of. Incompatible with `[lb_rank]`.
        - Optional, defaults to [lb_rank] OR yourself.
- `/guess leaderboard <guess_type> [page]` - View the guessing leaderboard.
    - `<guess_type>`: What type of guess.
    - `[page]`: What leaderboard page to view.
        - Optional, defaults to 1.
- `/guess jacket` - Guess the song based on the cropped jacket.
- `/guess jacket_smol` - Guess the song based on the super small (30px) cropped jacket.
- `/guess jacket_bw` - Guess the song based on the grayscale (black and white) cropped jacket.
- `/guess jacket_challenge` - Guess the song based on the super small (30px) grayscale (black and white) cropped jacket.
- `/guess character` - Guess the character based on the cropped 3*, 4*, or Birthday card.
- `/guess character_bw` - Guess the character based on the grayscale (black and white) cropped 3*, 4*, or Birthday card.
- `/guess chart` - Guess the song based on the cropped Master chart.
- `/guess chart_append` - Guess the song based on the cropped Append chart.
- `/guess event` - Guess the event based on the cropped event background.
- `/guess notes` - Guess the song based on the Master's note count.
### Other Fun Commands
- `/gacha [region] [reverse_odds]` - Simulate a 10 pull on the latest event gacha.
    - `[region]`: What region's gacha to use.
        - Optional, defaults to your default region (EN if not set).
    - `[reverse_odds]`: Whether to reverse 2* and 4* odds.
        - Optional, defaults to False.
- `/quiz` - Random PJSK quiz. NOT IMPLEMENTED
### Song Information Commands
- `/song info <song>` - View information about a specified song.
    - `<song>`: What song to view information of.
      - Mandatory.
- `/song chart <song> [difficulty]` - View the chart of a specified song.
    - `<song>`: What song to view chart of.
      - Mandatory.
    - `[difficulty]`: View chart of this difficulty.
      - Optional, defaults to Master.
- `/song jacket <song>` - View the jacket of a specified song.
    - `<song>`: What song to view the jacket of.
      - Mandatory.
- `/song strategy <song> [difficulty]` - View a strategy for the song, if exists.
    - `<song>`: What song to view a strategy guide for.
      - Mandatory.
    - `[difficulty]`: View strategy guide of this difficulty.
      - Optional, defaults to Master.
- `/song constant <song> [difficulty]` - View the constant (community-rated difficulty) of a specified song.
    - `<song>`: What song to view the constant of.
      - Mandatory.
    - `[difficulty]`: View constant of this difficulty.
      - Optional, defaults to Master.
      - Only supports Expert, Master, and Append.
> [!NOTE]  
> We do not support defining custom per-user aliases. Use these aliases anywhere in the bot that needs a song. Aliases are accepted in guessing, and all song parameters.
- `/song aliases <song>` - View defined aliases of a specified song.
    - `<song>`: What song to view aliases of.
      - Mandatory.
### Character Information Commands
- `/character info <character>` - View information about a specified PJSK character.
    - `<character>`: What character to view information on.
      - Mandatory.
> [!IMPORTANT]  
> The `<card>` parameter is a search bar! We support searching by rarity, attribute, character, and card name!
>
> For example, searching `3* cute haruka` will provide a list of autocompletes, all of which are [Cute] 3☆ Haruka Kiritani.
- `/character card <card>` - View information about a specified PJSK card.
    - `<card>`: What card to view information on.
      - Mandatory.
### Other Information Commands
- `/pjsk profile [user_id] [region]`
    - `[user_id]`: The user's ID. (same as friend ID)
        - Optional if your PJSK account is linked for specified region.
    - `[region]`: What region the account is from.
        - Optional, defaults to your default region (EN if not set).
- `/comics [region]`
    - `[region]`: What region's comics to use. The language will change accordingly.
        - Optional, defaults to your default region (EN if not set).
- `/pjsk why_inappropriate <text> [region]`
    - `<text>`: The text to check, to see why it's inappropriate on PJSK.
        - Mandatory.
    - `[region]`: What region's filter to use.
        - Optional, defaults to your default region (EN if not set).
### User Progression Commands
- `/b30 [region] [private] [filter]` - View the b30 plays (best 30 songs) of the account.
    - `[region]`: What linked account to view (eg. EN account b30).
      - Optional, defaults to ALL (merged from all your account data).
    - `[private]`: Hide the account ID and name.
       - Optional, defaults to False.
    - `[filter]`: What filters (FC only or AP only) to display the b30 with.
      - Optional, defaults to all (FC and AP).
- `/progress [difficulty] [region] [private]` - View a difficulty's progress, looking at FCs, APs, and Clears.
    - `[difficulty]`: View progress of this difficulty.
      - Optional, defaults to Master.
    - `[region]`: What linked account to view (eg. EN account progress)
      - Optional, defaults to your default region (EN if not set).
    - `[private]`: Whether to hide your PJSK name and ID, replacing it with your Discord name.
      - Optional, defaults to False.
- `/song progress <song> [region]` - View the progress of a specific PJSK song.
    - `<song>`: What song to view progress of.
      - Mandatory.
    - `[region]`: What linked account to view (eg. EN account song progress)
      - Optional, defaults to your default region (EN if not set).
- `/song difficulty <level>` - View all songs of a specified level.
    - `<level>`: What level to view songs of.
      - Mandatory.
### User Data/Setting Commands
> [!IMPORTANT]  
> Advanced command usage and information for some of these commands can be found at [LINKING](LINKING.md).
> This includes a "why" we need this data.

- `/user pjsk link [region]` - Link your PJSK account to your Discord account.
    - `[region]`: What the account's region is.
      - Optional, defaults to your default region (EN if not set).
- `/user pjsk unlink [region]` - Unlink your PJSK account from your Discord account.
    - `[region]`: What the account's region is.
      - Optional, defaults to your default region (EN if not set).
- `/user pjsk update_data [region]` - Update the stored user data. Requires a temporary account transfer.
    - `[region]`: What the account's region is.
      - Optional, defaults to your default region (EN if not set).
- `/user pjsk accounts` - View all linked account IDs.
- `/user settings` - Change Sbotga user settings.
### Sbotga Info Commands
- `/profile [user]` - View your profile, including level and Sbugacoin.
    - `[user]`: What user to view profile of.
        - Optional, defaults to yourself.
- `/xp_for <level>` - View the XP required for a specific level.
    - `<level>`: The level to view XP for.
- `/achievements [user]` - View your achievements in Sbotga.
    - `[user]`: What user to view profile of.
        - Optional, defaults to yourself.
### Uncategorized Commands
- `/help` - Sends you some basic information, as well as a link to this specific documentation page.
- `/donate` - Help support the bot. Sends you donation information.
- `/ping` - View Sbotga's latency.
