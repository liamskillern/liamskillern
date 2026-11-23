# Viral Indie Browser Games: Case Studies and Repeatable Patterns

Method note: page fetches were blocked in this session (Wikipedia, videogamecanon.com and krillion.io would not resolve). These findings come from search-result summaries of the cited pages, so treat each figure as "reported by" that source. Where sources disagree, the notes say so. Facts from memory that I could not re-source are marked UNVERIFIED and kept to Inferences/Gaps.

## Wordle: origin, growth timeline, emoji grid, NYT acquisition, aftermath

### Takeaway
Josh Wardle built Wordle as a gift for his partner. It went from about 90 players on Nov 1, 2021 to over 300,000 in early January 2022 and more than 2 million daily a few weeks later. The trigger was the spoiler-free emoji grid: players in New Zealand invented it, and Wardle added it as a native share button in December 2021. The New York Times bought the game on Jan 31, 2022 for "low seven figures", kept it free, and turned it into the anchor of NYT Games (4.8 billion plays in 2023).

### Cited Findings
- **Origin:** Wardle built it as a gift for his partner in October 2021. Some sources say he made an earlier prototype around 2011–2013 and abandoned it. Accounts conflict. — [theygotacquired.com](https://theygotacquired.com/gaming/wordle-acquired-by-the-new-york-times/); [UBC blog](https://blogs.ubc.ca/etec522/2023/06/05/founders-parade-josh-wardle-founder-of-wordle/); [Wikipedia: Josh Wardle](https://en.wikipedia.org/wiki/Josh_Wardle)
- **Growth:** about 90 players on Nov 1, 2021 (per NYT reporting). Over 300,000 by early January 2022, and more than 2 million daily "a few weeks later". Later sources cite about 10 million daily players after the sale. — [Wikipedia: Wordle](https://en.wikipedia.org/wiki/Wordle); [TIME interview](https://time.com/6143715/wordle-sale-josh-wardle-interview/); [wordplayforever history](https://wordplayforever.com/history)
- **Emoji grid:** players in New Zealand were sharing results as emoji, reportedly a woman named Elizabeth S. Wardle has said he did not invent the grid. In December 2021 he added a built-in "share" that copies the colored grid for Twitter. — [Wikipedia: Wordle](https://en.wikipedia.org/wiki/Wordle); [The Conversation](https://theconversation.com/wordle-how-a-simple-game-of-letters-became-part-of-the-new-york-times-business-plan-176299); [Slate interview with Wardle](https://slate.com/culture/2022/01/wordle-game-creator-wardle-twitter-scores-strategy-stats.html); [Know Your Meme](https://knowyourmeme.com/memes/subcultures/wordle)
- **Acquisition:** The NYT bought Wordle on Jan 31, 2022 for an "undisclosed price in the low-seven figures". It promised the game would stay free and that player streaks would carry over. — [TIME](https://time.com/6143715/wordle-sale-josh-wardle-interview/); [Wikipedia: Wordle](https://en.wikipedia.org/wiki/Wordle)
- **Aftermath:** Wordle was played 4.8 billion times in 2023 (Wikipedia). A less reliable site claims 5.3 billion in 2024. — [Wikipedia: Wordle](https://en.wikipedia.org/wiki/Wordle); [commandlinux stats](https://commandlinux.com/statistics/wordle-link/)
- The Conversation framed Wordle as part of the NYT's strategy of growing subscriptions through games and lifestyle products. — [The Conversation](https://theconversation.com/wordle-how-a-simple-game-of-letters-became-part-of-the-new-york-times-business-plan-176299)
- **Clone purge:** around Jan 11–12, 2022, Apple removed most Wordle copycat apps. Some had used the identical name and charged up to $30/year in subscriptions, or added ads and in-app purchases the original did not have. Sensor Tower data put the top 5 clones at about 176,000 App Store downloads. — [Engadget](https://www.engadget.com/wordle-clones-app-store-232042208.html); [Game Developer](https://www.gamedeveloper.com/game-platforms/-i-wordle-i-clones-nuked-from-ios-app-store); [PocketGamer.biz](https://www.pocketgamer.biz/apple-shuts-down-wordle-clones-on-app-store); [Bloomberg](https://www.bloomberg.com/news/articles/2022-01-12/apple-removes-wordle-apps-after-user-confusion-stokes-downloads)

### Inferences
- What made Wordle work was scarcity: one puzzle a day that everyone shares. That makes it a shared daily conversation topic. The spoiler-free grid turned each player's result into an ad without giving away the answer.
- Wardle never monetized it (no ads). Its "brand purity" was part of why the clones that charged money drew backlash, and arguably part of why it sold. The NYT valued it as a subscription funnel, not as ad inventory.
- The main share feature came from users, so watching how players already share is a good source of design ideas.

### Gaps
- I could not fetch NYT Games subscriber totals for after the acquisition from a primary source.
- The exact date the share button went live (mid-December 2021) is not confirmed to the day.
- UNVERIFIED from memory: Wordle Archive was taken down after the NYT acquisition, and Hasbro released a Wordle party board game in 2022. Neither is cited here.

## Other hits and how they spread

### Takeaway
The hits split into three groups.
1. **Wordle-format reskins for a niche fandom** (Heardle for music, Worldle/Globle for geography, Framed for film). These spread through the same share-grid mechanic, and the best of them were bought or grew into small studios.
2. **Weekend-built "toy" web games with surprising escalation** (2048, Infinite Craft, Password Game, Universal Paperclips, A Dark Room, Cookie Clicker). These spread through social media, Hacker News, Reddit and streamers.
3. **Real-time multiplayer .io games** (Agar.io, Slither.io). These spread through YouTubers and 4chan/Reddit and made money from ads at very large scale.

### Cited Findings

**Heardle (music, 2022)**
- Created by Glenn Angelo of London design studio Studio Omakase, who was anonymous at first and identified via a Product Hunt post. Spotify announced the acquisition on July 12, 2022; the price was undisclosed. — [TechCrunch](https://techcrunch.com/2022/07/12/spotify-acquired-heardle-wordle-music-game); [Axios](https://www.axios.com/2022/07/12/spotify-acquire-heardle-music-trivia-game); [Rolling Stone](https://www.rollingstone.com/music/music-news/spotify-buys-heardle-music-game-1381438/); [Digital Music News](https://www.digitalmusicnews.com/2022/07/12/heardle-spotify-acquisition/)
- Spotify shut Heardle down in April 2023 "to prioritize other means of music discovery". — [Wikipedia: Heardle](https://wikipedia.com/wiki/Heardle)

**Worldle / Globle / Framed (geography and film, 2022)**
- Worldle was created by Antoine Teuf (@teuteuf) in early January 2022 as a side project. He called it a "tribute" to Wordle (Washington Post interview). — [Wikipedia: Worldle](https://en.wikipedia.org/wiki/Worldle)
- Worldle grew into Teuteuf Games, a daily geography game studio based in Ireland and the USA. Its titles include Travle, Flagle, Statele, GeoGrid, WhereTaken and WhenTaken. It launched WhenTaken Movies in January 2025. — [Teuteuf team page](https://teuteuf.fr/team/); [press release](https://markets.financialcontent.com/concordmonitor/article/globeprwire-2025-1-16-worldle-creators-launch-whentaken-movies-a-new-daily-geography-game-for-movie-lovers)
- Globle was created by "The Abe Train" in 2022. A third-party clone site claims "800K+ players", which is unreliable. — [progameguides](https://progameguides.com/wordle/what-is-globle-a-wordle-geography-game/); [wordle.global](https://wordle.global/en/globe)
- Framed (framed.wtf) shows a movie still and has players guess the film. Its creator stayed anonymous at launch. — [Rolling Stone UK](https://rollingstone.co.uk/culture/wordle-inspired-game-framed-challenges-film-buffs-13584); [GameSpot](https://www.gamespot.com/articles/framed-is-a-wordle-like-with-scenes-from-movies/1100-6501819/)

**Connections (NYT, 2023): not indie, but shows where the format went**
- Beta launched June 12, 2023. Puzzle editor Wyna Liu got the project after it came out of an internal NYT Game Jam. The NYT called it its most successful in-house launch since the Mini Crossword (2014) and its second most-played game after Wordle, but gave no user numbers. — [TechCrunch](https://techcrunch.com/2023/08/28/connections-is-the-new-york-times-most-played-game-after-wordle); [Wikipedia: Connections](https://en.wikipedia.org/wiki/The_New_York_Times_Connections)
- A blog claims "3.3 billion plays in 2024". This is unverified. — [thewordfinder blog](https://www.thewordfinder.com/blog/?p=1604)

**Neal Agarwal / neal.fun (Infinite Craft, The Password Game)**
- Infinite Craft launched Jan 31, 2024. It is an LLM-backed crafting game that starts with water, fire, wind and earth. By Feb 2, 2024, players were making about 1,000 crafts per second, and Agarwal publicly asked his AI provider to raise the rate limit. The iOS version followed around Apr 27–30, 2024 and Android on May 21, 2024. — [Wikipedia: Infinite Craft](https://en.wikipedia.org/wiki/Infinite_Craft); [Know Your Meme](https://knowyourmeme.com/memes/sites/infinite-craft); [PC Gamer](https://www.pcgamer.com/this-browser-based-endless-crafting-game-starts-you-off-with-fire-and-water-but-it-quickly-escalates-to-god-the-big-bang-and-yin-yoda)
- One launch post got about 21M impressions. neal.fun is reported to get about 2M players/month, a figure from a secondary Substack. — [gameplaydev Substack](https://gameplaydev.substack.com/p/this-solo-web-game-dev-went-viral)
- The Password Game launched June 27, 2023 after about two months of development. It parodies password rules. It spread through rule previews on X, TikTok clips, YouTube speedruns and a disclosed collaboration with streamer Kitboga, who got scammers to play it. It reportedly passed 10M page views by October. Another source claims "30k views in first month", which is irreconcilable with that. — [Wikipedia: The Password Game](https://en.wikipedia.org/wiki/The_Password_Game); [howitspread](https://howitspread.com/cases/the-password-game); [Kitboga on X](https://x.com/Kitboga/status/1682134939368554501); [Quartz](https://qz.com/password-game-internet-security-neal-agarwal-1850590337)
- Agarwal reportedly made a full-time living from neal.fun ad revenue by the time he graduated from Virginia Tech. Other sources mention sponsorships, Patreon or tips. No figures are public. — [Wikipedia: Neal Agarwal](https://en.wikipedia.org/wiki/Neal_Agarwal); [WeGotThisCovered](https://wegotthiscovered.com/gaming/what-is-the-password-game-on-neal-fun-the-internets-newest-viral-browser-game/); [Arc interview](https://arc.net/blog/a-convo-w-neal-agarwal)

**Universal Paperclips (Frank Lantz, 2017)**
- A free browser incremental game about an AI paperclip maximizer, made by Frank Lantz in 2017. It now has an official $1.99 mobile app. Lantz has not disclosed revenue. — [Wikipedia: Universal Paperclips](https://en.wikipedia.org/wiki/Universal_Paperclips); [IF50 / Aaron Reed](https://if50.substack.com/p/2017-universal-paperclips); [App Store](https://apps.apple.com/us/app/id1300634274); [dinogame.gg](https://dinogame.gg/blog/browser-games-that-earned-over-million/)

**A Dark Room (Michael Townsend, 2013)**
- A free text-based browser game from 2013. The iOS port (by Amir Rajan) topped the US paid App Store chart for most of April 2014, with about 325,000 downloads by the end of that month (roughly $250k). A two-year postmortem reported $697,270 gross revenue. — [Game Developer postmortem](https://gamedeveloper.com/business/a-two-year-look-at-the-sales-of-chart-topping-ios-title-i-a-dark-room-i-); [Cult of Mac](https://www.cultofmac.com/?p=274582)

**Cookie Clicker (Julien "Orteil" Thiennot, 2013)**
- A free browser game. Orteil reported a traffic peak of 1.5M hits in one day in August 2013. — [dinogame.gg](https://dinogame.gg/blog/browser-games-that-earned-over-million/)
- The Steam release in September 2021 hit an all-time peak of 67,867 concurrent players on Sep 12, 2021, more than Rainbow Six Siege and Civ 6 at the time. It has about 96–97% positive reviews from around 80k reviews. A claim of "$500k in first days" comes only from an unsourced forum post. — [SteamDB](https://steamdb.info/app/1454400/graphs); [PC Gamer](https://www.pcgamer.com/more-people-playing-cookie-clicker-than-rainbow-six-siege-civ-6-phasmophobia); [NME](https://www.nme.com/news/cookie-clicker-has-quickly-become-one-of-the-most-popular-games-on-steam-3038588); [Unity forum](https://discussions.unity.com/t/the-new-cookie-clickers-phenomenal-success/854845)

**Agar.io and Slither.io (.io games, 2015–2016)**
- Matheus Valadares (19, Brazil) announced Agar.io on 4chan on Apr 27, 2015. Miniclip acquired the publishing rights within about a week, when the game already had "millions of daily players". Mobile ports followed around July 2015. Valadares later made Diep.io (2016). — [Wikipedia: .io games](https://en.wikipedia.org/wiki/.io_games); [GamesBeat](https://gamesbeat.com/the-surprising-momentum-behind-io-games-like-agar-io/); [Wikipedia: Diep.io](https://Www.wikipedia.org/wiki/Diep.io)
- Slither.io (Steve Howse, 2016, inspired by Agar.io) reportedly earned about $100,000 a day at its 2016 peak. The money came from ads shown after death plus a $3.99 ad-free option. Servers reportedly cost about $15k/month. — [Digital Trends](https://www.digitaltrends.com/gaming/viral-app-slither-pulls-100k-per-day/); [Loop Insight](https://www.loopinsight.com/2016/06/20/slither-io-game-goes-viral-brings-developer-100k-a-day/); [Root-Nation](https://root-nation.com/en/games-en/games-articles-en/en-slither-io-and-agar-io-behind-the-game-scene/)

**2048 (Gabriele Cirulli, March 2014)**
- A 19-year-old built it in one weekend to test whether he could write a game from scratch. It got more than 4M visitors in under a week and 33M+ plays (City AM). It is a "clone of a clone": the README credits 1024 by Veewo, which is "conceptually similar to Threes". It was open source, which led to countless variants. By April 2014 about 15 Threes clones a day were appearing on the App Store. — [City AM](https://www.cityam.com/how-one-19-year-old-won-internet-addictive-puzzler-2048/); [Wikipedia: 2048](https://en.wikipedia.org/wiki/2048_(video_game)); [Daily Dot](https://dailydot.com/threes-2048-app-strategy-history); [Business Insider](https://www.businessinsider.in/puzzle-game-2048-will-make-you-forget-flappy-bird-ever-existed/amp_articleshow/32559256.cms)

**Suika (watermelon merge) browser clones**
- The concept comes from the Chinese browser game Merge Big Watermelon (January 2021). Japanese streamers and VTubers drove a revival from May 2023, and it reached #82 most-watched on Twitch in September 2023. Aladdin X's official Switch version came out globally on Oct 20, 2023. Dozens of free HTML5 clones followed on itch.io and GitHub (matter.js, Phaser), including themed variants (Pokémon, Touhou). — [Wikipedia: Suika Game](https://wikipedia.com/wiki/Suika_Game); [TouchArcade](https://toucharcade.com/2023/10/11/how-to-play-suika-watermelon-game-free-on-mobile-browser-iphone-android/); [itch.io tag](https://itch.io/games/html5/tag-suika-game); [LevelUp](https://www.levelup.com/en/news/there-is-a-free-to-play-version-of-suika-game-that-you-can-play-in-your-browser/)

**LinkedIn Queens (2024)**
- LinkedIn launched Queens, Crossclimb and Inference on May 1, 2024 to increase time spent on the platform. Thomas Snyder, a three-time World Sudoku Champion, leads the effort as "Principal Puzzle Master". He says every puzzle is written by a human. — [TechCrunch](https://techcrunch.com/2024/05/01/linkedin-launches-gaming-three-logic-puzzles-aiming-to-extend-time-spent-on-its-networking-platform); [Entrepreneur](https://www.entrepreneur.com/business-news/heres-how-hes-shaping-linkedins-puzzle-game); [Beebom interview](https://beebom.com/puzzle/linkedin-games-thomas-snyder-interview/)
- Hacker News commenters identify Queens as an easier version of the classic "Star Battle" logic puzzle (one star per row, column and region, no two touching). This is community opinion, not a LinkedIn statement. — [HN thread](https://hn.svelte.dev/item/44275900)

**2025–2026 viral indie web games, including Krillion**
- Krillion (krillion.io) is a daily trivia game with seven prompts at 25 seconds each. Rarer valid answers score higher ("sink deeper"). Reported launch dates and creators conflict: one source says July 9, 2026 by a 22-year-old solo developer called "kp", another says August 2026 by "Jing Lee", and IGDB lists July 15, 2026. All of these are aggregator or fan sites. — [krillionguide](https://krillionguide.com/en/similar-games); [wordlewebsite](https://wordlewebsite.com/krillionio); [IGDB](https://www.igdb.com/games/krillion); [zapgames](https://zapgames.io/krillion-game)
- Reported spread: Krillion is said to be #1 on the "Playlin 40" weekly daily-web-game chart (Chart #18, Sept 2026). Fan Minecraft variants followed (Minellion by YouTuber Hydro, playkrillion.net/minecraft, krillion.cc), and Beebom covered a Minecraft Krillion. Bisect Hosting lists it among the most addictive daily games of 2026. — [Endgame Tools](https://endgametools.com/en/minecraft/news/minecraft-krillion); [Beebom](https://beebom.com/minecraft-krillion-trivia-game-launched/amp/); [Bisect Hosting](https://www.bisecthosting.com/blog/five-addicting-daily-puzzle-games-in-2026-dle-minecraftle-krillion-more)
- Pieter Levels' fly.pieter.com (2025) is a multiplayer browser flight simulator built largely with AI prompting that went viral. Megabonk (2025) was a viral solo hit, but on PC/Steam rather than in the browser. — [gameplaydev / search summary](https://gameplaydev.substack.com/p/this-solo-web-game-dev-went-viral); [Wikipedia: Megabonk](https://en.wikipedia.org/wiki/Megabonk)

### Inferences
- **The "-dle" template is a format, not a game.** Take one daily answer, add limited guesses with feedback and a shareable spoiler-free result, then point it at a fandom. Heardle, Worldle, Globle, Framed and now Krillion all follow it. Krillion's twist is scoring by answer rarity instead of correctness, which is close to Family Feud played in reverse.
- **Toy games spread through screenshots of surprising output.** Infinite Craft's absurd combinations, Password Game's rules and 2048's tile numbers are all highly screenshot-able.
- **Streamers are a growth channel of their own.** Suika (VTubers), Password Game (Kitboga) and Agar.io/Slither.io (YouTubers) all hit their peaks through creators.

### Gaps
- No primary daily-player figures for Heardle, Globle or Framed. Framed's creator is not reliably identified in my results.
- No player numbers for Universal Paperclips. A widely repeated figure is "450k players in its first 11 days" (UNVERIFIED; no source found).
- Who designed Queens, and whether LinkedIn explicitly cites Star Battle, remain unconfirmed.
- Krillion's creator, launch date and traffic could not be verified from a primary source; krillion.io was unreachable.
- I did not research browser Flappy Bird clones specifically. UNVERIFIED context: Flappy Bird was a mobile game pulled by Dong Nguyen in February 2014, which triggered a wave of web and app clones.

## What patterns repeat

### Takeaway
Most hits pair a known mechanic (Mastermind/Lingo, Threes, Star Battle, merge puzzles, crafting games) with one twist, ship it free in the browser with no sign-up, and include a built-in reason to share. The daily cadence creates appointment play and a shared conversation. Niche fandoms (music, geography, film, Minecraft) make reskins of a proven format spread within their communities. Launch channels vary: Twitter/X (Wordle), 4chan (Agar.io), Product Hunt (Heardle), X plus TikTok and streamers (Password Game, Suika). Many came from people with existing audiences or distribution (Agarwal, Levels, Lantz).

### Cited Findings
- 2048 was built in a weekend from an existing concept (1024/Threes) and reached 4M visitors in under a week. — [City AM](https://www.cityam.com/how-one-19-year-old-won-internet-addictive-puzzler-2048/)
- Wordle's share grid came from users and turned results into spoiler-free social posts. — [The Conversation](https://theconversation.com/wordle-how-a-simple-game-of-letters-became-part-of-the-new-york-times-business-plan-176299)
- Worldle's creator called it a "tribute" adapting Wordle to geography, and it grew into a studio of daily geography games. — [Wikipedia: Worldle](https://en.wikipedia.org/wiki/Worldle); [Teuteuf](https://teuteuf.fr/team/)
- Agar.io was announced on 4chan. — [Wikipedia: .io games](https://en.wikipedia.org/wiki/.io_games)
- Heardle's creator surfaced on Product Hunt. — [Axios](https://www.axios.com/2022/07/12/spotify-acquire-heardle-music-trivia-game)
- The Password Game spread through X previews, TikTok, speedruns and a streamer collaboration. — [howitspread](https://howitspread.com/cases/the-password-game)
- Suika's 2023 surge was driven by Japanese VTubers and streamers. — [Wikipedia: Suika Game](https://wikipedia.com/wiki/Suika_Game)
- Infinite Craft's launch post got about 21M impressions, and the creator already had an established site (neal.fun). — [gameplaydev Substack](https://gameplaydev.substack.com/p/this-solo-web-game-dev-went-viral)
- The rise of daily ".io" trivia games since early 2026 is credited partly to Krillion. — [Wikipedia: .io games](https://en.wikipedia.org/wiki/.io_games) (via search summary)

### Inferences
- **Repeatable recipe for a solo developer:**
  1. Pick a proven mechanic.
  2. Add one twist or a fandom-specific dataset.
  3. Load instantly on mobile web with no account.
  4. Offer one daily challenge or a short session.
  5. Build in a share artifact that reveals performance but not the answer.
  6. Seed it to the target community (subreddit, Discord, X, a TikTok or streamer).
- **Timing matters.** The 2022 wave of Wordle variants rode Wordle's peak attention, and the Suika clones rode the Switch launch and streamer hype.
- **Novelty plus readability.** Players should understand the game in one screenshot.

### Gaps
- I did not find documented Hacker News launch threads with metrics for these games. HN is commonly cited for 2048 and neal.fun, but this is UNVERIFIED here.

## Outcomes: acquisitions, ad revenue, Patreon, Steam and mobile, or fading

### Takeaway
Outcomes fall into four groups.
- **Acquisition:** Wordle for low-seven figures to the NYT; Heardle to Spotify (price undisclosed, shut down 9 months later); Agar.io publishing rights to Miniclip.
- **Ad revenue at scale:** Slither.io at about $100k/day at its peak; neal.fun as a full-time living.
- **Premium ports of a free web original:** A Dark Room iOS at about $697k gross over two years; Cookie Clicker on Steam at a 67.9k concurrent peak; Universal Paperclips mobile at $1.99; Infinite Craft mobile.
- **Growing into a studio:** Teuteuf Games.

Many clones and minor variants faded once the trend passed.

### Cited Findings
- Wordle: NYT, low-seven figures, Jan 31, 2022. — [TIME](https://time.com/6143715/wordle-sale-josh-wardle-interview/)
- Heardle: Spotify, July 2022, undisclosed; shut down April 2023. — [TechCrunch](https://techcrunch.com/2022/07/12/spotify-acquired-heardle-wordle-music-game); [Wikipedia: Heardle](https://wikipedia.com/wiki/Heardle)
- Agar.io: Miniclip got publishing rights within about a week of launch. — [GamesBeat](https://gamesbeat.com/the-surprising-momentum-behind-io-games-like-agar-io/)
- Slither.io: about $100k/day from ads and a $3.99 ad removal at its 2016 peak. — [Digital Trends](https://www.digitaltrends.com/gaming/viral-app-slither-pulls-100k-per-day/)
- A Dark Room iOS: about 325k downloads and about $250k in April 2014; $697,270 gross over two years. — [Game Developer](https://gamedeveloper.com/business/a-two-year-look-at-the-sales-of-chart-topping-ios-title-i-a-dark-room-i-)
- Cookie Clicker Steam: all-time concurrent peak of 67,867 on Sept 12, 2021. — [SteamDB](https://steamdb.info/app/1454400/graphs)
- neal.fun: full-time living from ads, plus reported sponsorships and Patreon. — [Wikipedia: Neal Agarwal](https://en.wikipedia.org/wiki/Neal_Agarwal); [WeGotThisCovered](https://wegotthiscovered.com/gaming/what-is-the-password-game-on-neal-fun-the-internets-newest-viral-browser-game/)
- Universal Paperclips: official mobile app for $1.99; revenue undisclosed. — [App Store](https://apps.apple.com/us/app/id1300634274); [dinogame.gg](https://dinogame.gg/blog/browser-games-that-earned-over-million/)
- Infinite Craft: iOS (late April 2024) and Android (May 21, 2024) versions. — [Wikipedia: Infinite Craft](https://en.wikipedia.org/wiki/Infinite_Craft)
- Teuteuf: grew into a multi-game studio and was still launching titles in 2025. — [press release](https://markets.financialcontent.com/concordmonitor/article/globeprwire-2025-1-16-worldle-creators-launch-whentaken-movies-a-new-daily-geography-game-for-movie-lovers)

### Inferences
- An acquisition does not guarantee the game survives: Heardle was shut down about 9 months after Spotify bought it. Wordle survived because it fit the NYT's subscription bundle.
- For solo developers, the more durable options are a portfolio site like neal.fun or a studio of daily games like Teuteuf, which turns one hit into steady traffic. A free web version plus a paid port (Steam or mobile) is a proven path.
- Slither.io's revenue came with large server costs, so real-time multiplayer is a much higher-cost bet than a static daily puzzle.

### Gaps
- No public sale price for Heardle or for the Agar.io/Miniclip deal, and no official Cookie Clicker Steam sales numbers.
- No Patreon figures found for any of these developers.

## Why copycats and clones failed

### Takeaway
Clones that only copied the surface failed for three reasons: platforms removed them (Apple purged Wordle clones in January 2022), the community turned against them for monetizing a free, ad-free original, or they added no new twist and were drowned out (about 15 Threes clones a day; dozens of near-identical Suika clones and Steam idle games). Clones that succeeded, such as 2048, Worldle and Slither.io, either executed better, offered a free alternative to a paid original, or retargeted the format to a new niche.

### Cited Findings
- Apple removed Wordle copycat apps on Jan 11–12, 2022 after backlash. Some used the exact name and charged up to $30/year, with ads and IAPs the original lacked. One clone's creator publicly apologized ("I f—ed up"). — [Engadget](https://www.engadget.com/wordle-clones-app-store-232042208.html); [Yahoo News](https://news.yahoo.com/creator-wordle-ripoff-app-apologizes-064353000.html); [Euronews](https://www.euronews.com/2022/01/12/wordle-copycat-apps-taken-off-app-store-after-online-criticism)
- The top 5 Wordle clones together drew only about 176k downloads. — [PocketGamer.biz](https://www.pocketgamer.biz/apple-shuts-down-wordle-clones-on-app-store)
- About 15 new Threes clones a day hit the App Store in April 2014, and 2048, the free web clone, overshadowed the paid original. — [Wikipedia: 2048](https://en.wikipedia.org/wiki/2048_(video_game)); [Daily Dot](https://dailydot.com/threes-2048-app-strategy-history)
- In one week, 54 idle games were released on Steam, and "many look eerily similar". — [PC Gamer](https://pcgamer.com/gaming-industry/steam-week-in-review-54-idle-games-released-on-steam-last-week-and-many-look-eerily-similar)
- Agar.io was itself followed by Slither.io, which succeeded by changing the core mechanic (snake versus cell). — [Wikipedia: Slither.io](https://en.wikipedia.org/wiki/Slither.io)

### Inferences
- **Failure modes:** an identical name or branding, which brings platform and trademark risk; aggressive monetization of something people know as free; no fandom or twist; arriving after peak attention; and weak social sharing.
- **Success modes for derivatives:** a new niche dataset, a changed core rule (rarity scoring, snake versus blob), or being free and web-first where the original was paid or app-only.

### Gaps
- No systematic data on the survival rates of "-dle" variants. Lists like the Playlin 40 chart might provide it, but they were not reachable.
