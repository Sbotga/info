- **日本語**
# コマンド一覧 (工事中)
Sbotgaは様々なコマンドがあります！ここに全てのコマンドと内容が見つかります。

`<argument>` - 当てはめるのが必須な空欄。

`[argument]` - 当てはめるのが任意な空欄。

> [!NOTE]  
> `song`の自動補完にはローマ字に変換した曲と略は入っていません。だが, どっちも認識はします。
> 
> `song`と`character`は "fuzzy match" (当てはめた言葉に一番近い曲名) をしようとします. (誤字をしても大丈夫。)
### ランクマッチ用コマンド
- `/ranked view [rank] [region]` - 現在のシーズンのTOP100の詳細を見る。
    - `[rank]`: どの順位を見るか
        - もしアカウントがTOP100でbotと連携してたら任意。
    - `[region]`: どのリージョンを見るか。
        - 任意、グローバルにデフォルト。
- `/ranked leaderboard [region]` - 現在のシーズンのTOP100を見る。
    - `[region]`: どのリージョンを見るか。
        - 任意、グローバルにデフォルト。
### イベント用コマンド
- `/event view [rank] [region] [character]` - 現在のイベントのTOP100の詳細を見る。
    - `[rank]`: どの順位を見るか
        - もしアカウントがTOP100でbotと連携してたら任意。
    - `[region]`: どのリージョンを見るか。
        - 任意、グローバルにデフォルト。
    - `[character]`: どのチャプターか（ワールドリンクの場合）
        - 任意。
- `/event leaderboard [region] [character]` - 現在のイベントのTOP100を見る。
   - `[rank]`: どの順位を見るか
        - もしアカウントがTOP100でbotと連携してたら任意。
    - `[region]`: どのリージョンを見るか。
        - 任意、グローバルにデフォルト。
### クイズ用コマンド (TODO)
> [!IMPORTANT]  
> クイズ用コマンドは仕組みによりサーバーでしかコマンドが使えません。順位とは詳細はどこでも使えます（DMでも）。
- `/guess hint` - 今のクイズに関してヒントをもらう。
- `/guess end` - 今のクイズを終わらせる。
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
- `/guess jacket_challenge` - Guess the song based on the super small (30px) grayscale (black and white) cropped jacket. UNRANKED!
- `/guess character` - Guess the character based on the cropped 3*, 4*, or Birthday card.
- `/guess character_bw` - Guess the character based on the grayscale (black and white) cropped 3*, 4*, or Birthday card.
- `/guess chart` - Guess the song based on the cropped Master chart.
- `/guess chart_append` - Guess the song based on the cropped Append chart.
