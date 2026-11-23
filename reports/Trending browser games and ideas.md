# Build small daily games that spread

**The short version.** The hottest browser games in late 2026 are short daily games where everyone gets the same puzzle, play takes about three minutes, and you can share your result without giving away the answer. The breakout this year is **Krillion**, a daily trivia game where *rarer* correct answers score more points. It has been #1 on an independent weekly chart of daily web games for 15 weeks ([Playlin 40](https://playlin.io/charts/)), but almost nothing about it (creator, launch date, player count) is confirmed by a first-hand source. Wordle is still huge, about 4.2 billion solves in 2025 ([NBC New York](https://www.nbcnewyork.com/entertainment/entertainment-news/hardest-wordle-connections-games-2025/6436464/)), but the newest energy is in logic puzzles, geography games, and trivia scored "on a scale" instead of right/wrong. What makes these games addictive is a small, well-understood set of mechanics: one puzzle a day, streaks, a spoiler-free share result, instant restarts, and satisfying feedback. Each one can be built by a beginner. Solo developers have built hits in a weekend (2048) or three days (Actorle, still earning about $4,000/month two years later, self-reported) ([City AM](https://www.cityam.com/how-one-19-year-old-won-internet-addictive-puzzler-2048/); [Indie Hackers](https://www.indiehackers.com/post/how-did-i-create-a-game-with-4-000-monthly-revenue-in-3-days-49b598a252)). Most indie web games earn little, though, and getting players is harder than building the game. Below are 10 original ideas sized for a solo beginner. Two fit a cybersecurity background. A one-to-two-week plan to ship the first one closes the report.

---

## What is trending right now (late 2026)

### Daily games dominate, and small indie developers are winning

An independent weekly chart of daily web games, the Playlin 40, gives the best current snapshot. For the week of Nov 16, 2026 it ranked ([Playlin 40](https://playlin.io/charts/)):

| Rank | Game | Note |
|---|---|---|
| 1 | Krillion | 15 weeks on chart |
| 2 | Size It Up | indie |
| 3 | Extraplot | new entry |
| 4 | Layers | indie |
| 5 | Number Waffle | indie |
| 22 | Wordle | NYT |
| 26 | Connections | NYT |
| 31 | MapTap | geography daily |

**Caveat:** Playlin is a small aggregator. It counts plays among its own users, not the whole internet, and its method is unknown. Wordle sitting at #22 does not mean Wordle is shrinking. It means indie games are hot *on that site*. The research also couldn't confirm what most of the top-5 games actually are.

### Other games worth knowing

| Game | What it is | Why it matters to you |
|---|---|---|
| **Wordle** (NYT) | Guess a 5-letter word in 6 tries, once a day | Still the template. About 4.2B solves in 2025 ([NBC New York](https://www.nbcnewyork.com/entertainment/entertainment-news/hardest-wordle-connections-games-2025/6436464/)) |
| **Pips** (NYT, Aug 2025) | Domino-placement logic puzzle | 612M solves in 2025 ([NBC New York](https://www.nbcnewyork.com/entertainment/entertainment-news/hardest-wordle-connections-games-2025/6436464/)): logic puzzles are rising |
| **LinkedIn games** | 8 daily puzzles, including Queens, Zip, Patches (Mar 2026), Wend (Jun 2026) | LinkedIn is shifting from word to logic puzzles ([GamesBeat](https://gamesbeat.com/?p=319165); [LinkedIn](https://news.linkedin.com/2026/LinkedIn-AnnouncesWend)) |
| **Clues by Sam** | Daily logic deduction | 50,000+ daily players by early 2026 ([Wikipedia](https://en.wikipedia.org/wiki/Clues_By_Sam)) |
| **MapTap** | Tap 5 places on a 3D globe, scored by distance | A TechCrunch writer called it "my new Wordle" ([TechCrunch](https://techcrunch.com/2026/06/18/maptap-a-daily-geography-game-is-my-new-wordle)) |
| **Boreen** | Irish daily trivia spreading via WhatsApp, compared to Krillion | Shows the Krillion format being localized ([Irish Times](https://irishtimes.com/life-style/people/2026/11/22/whats-the-story-with-boreen-the-daily-irish-trivia-game), search snippet only) |
| **Your AI Slop Bores Me** (Mar 2026) | Humans pretend to be an AI answering other people's prompts | Viral via Hacker News, rides anti-AI sentiment ([Kotaku](https://kotaku.com/ai-llm-slop-new-free-game-2000677087)) |
| **Messenger** (Abeto) | Cozy WebGL mail delivery on a tiny planet, with other live players visible | Went viral again in June 2026 ([Aftermath](https://aftermath.site/messenger-browser-game-abeto)) |
| **Destroy Any Website** (Sep 2026) | Turns any URL into a destructible level | One-sentence hook ([aiidelist](https://aiidelist.com/blog/destroy-any-website), secondary source) |

### Krillion: what is known and what isn't

**What multiple sources agree on:** each day there are seven prompts shared by every player, with about 20–25 seconds each. You type your own answers. Valid but *rare* answers score more, framed as diving deeper into the ocean, and the top tier is "One in a Krillion" ([Game Rant](https://gamerant.com/krillion-answers-today-november-23-dive-131/); [TechWiser](https://techwiser.com/krillion-answers-today/)). Dive #131 fell on Nov 23, 2026 ([Game Rant](https://gamerant.com/krillion-answers-today-november-23-dive-131/)). Student newspapers describe it spreading through classrooms ([Scot Scoop](https://scotscoop.com/krillion-takes-a-dive-into-classroom-games/); [IBW Headlight](https://ibwheadlight.com/7600/artsentertainment/krillion-is-this-the-new-big-game/)).

**What is weakly sourced or conflicting (treat as unverified):**

- **Creator:** most sources say a pseudonymous solo developer called "kp", and one says "Jing Lee". All of these are fan or SEO sites ([krilliondaily](https://krilliondaily.com/blog/who-made-krillion); [krillionguide](https://krillionguide.com/en/similar-games)).
- **Launch date:** sources give July 9, July 15 or August 2026 ([IGDB](https://www.igdb.com/games/krillion); [zapgames](https://zapgames.io/krillion-game)).
- **Player count:** "hundreds of thousands daily, if not millions" is a student newspaper's guess, not a developer figure ([IBW Headlight](https://ibwheadlight.com/7600/artsentertainment/krillion-is-this-the-new-big-game/)).
- **Business model:** one guide site says the daily dive is free and endless mode plus archive is a one-time $5 unlock ([dailydles](https://dailydles.com/games/krillion)). Another says it's simply free.
- **Official site:** krillion.io appears to be the original. Many look-alike domains exist, and at least one says it's unaffiliated ([krillion.org](https://www.krillion.org/)).

The flood of clone and "answers today" sites is itself evidence of big search demand. It's also a warning: copying a hot game's name gets you lost in that crowd.

### Where browser games get played

| Channel | Best for | Key fact |
|---|---|---|
| **Your own domain** | Daily puzzles | Discovery comes from shared results, group chats and classrooms |
| **Poki / CrazyGames** | Arcade and action games | Poki claims 100M+ monthly players ([Poki report](https://poki.com/blog/state-of-web-gaming-report-2026), self-reported) |
| **YouTube Playables** | Brain and puzzle games | 1,669 games; puzzle games get 23.6% of plays ([Dubit](https://dubit.io/library/how-many-plays-does-a-youtube-playables-game-get)). Revenue share is still invite-only ([Google](https://developers.google.com/youtube/gaming/playables/reference/monetization)) |
| **Reddit (Devvit)** | Daily games with built-in community | Ran a "Game of the Day 2026" hackathon and a $40K Phaser hackathon ([Phaser](https://phaser.io/news/2026/06/reddit-and-phaser-launch-a-40-000-game-dev-hackathon)) |
| **Telegram "tap-to-earn"** | Avoid | Hamster Kombat lost ~86% of users by Nov 2024 ([Cointelegraph](https://cointelegraph.com/news/hamster-kombat-decline-telegram-game-competition-rise-of-paws)) |

---

## What makes a browser game addictive

Seven mechanics come up again and again. You don't need all of them. The best small games combine three or four.

| # | Mechanic | Plain-language meaning | Evidence |
|---|---|---|---|
| 1 | **One shared puzzle a day** | Everyone plays the same thing today, and then it's gone until tomorrow | Wordle's 2013 prototype had unlimited play. The once-a-day limit came with the 2021 hit ([PocketGamer.biz](https://www.pocketgamer.biz/news/78481/gdc-josh-wardle-shares-his-incorrect-tips-for-wordles-success/)). Psychologists call this scarcity ([SNHU](https://www.snhu.edu/about-us/newsroom/hot-topics/psychology-of-wordle)) |
| 2 | **Streaks** | A counter of how many days in a row you've played | Duolingo users with a 7-day streak are 2.4x more likely to return the next day ([Duolingo](https://blog.duolingo.com/how-duolingo-streak-builds-habit)). One hard Wordle word broke 5.6M streaks ([TODAY via AOL](https://www.aol.com/exclusive-wordle-puzzle-ended-5-013624721.html)) |
| 3 | **Spoiler-free share result** | A copyable result (like Wordle's emoji grid) that shows *how* you did without the answer | Wordle went from ~90 players (Nov 2021) to 300K (early Jan 2022) to 2M+ a week later, right after the share grid shipped ([World Economic Forum](https://www.weforum.org/stories/all/wordle-game-new-york-times-business-plan/); [NPR](https://www.npr.org/2022/01/14/1072980440/a-simple-word-game-is-the-newest-social-media-phenomenon)). A player invented the grid, not the developer ([Know Your Meme](https://knowyourmeme.com/memes/subcultures/wordle)) |
| 4 | **Scoring on a scale, not pass/fail** | You score 0–100 (distance, rarity, depth), so every result is different and worth comparing | Krillion (rarity) and MapTap (distance) both work this way. This pattern is inferred from how those games are described |
| 5 | **Brag-worthy rare moments** | Rare outcomes you want to screenshot | Infinite Craft's "First Discovery" credits you for being first to craft something ([PC Gamer](https://www.pcgamer.com/this-browser-based-endless-crafting-game-starts-you-off-with-fire-and-water-but-it-quickly-escalates-to-god-the-big-bang-and-yin-yoda)). Krillion's "One in a Krillion" tier works the same way |
| 6 | **"One more try"** | Instant restart, short runs, and a visible "so close" | Near-misses increase the urge to keep playing, especially when the player feels in control ([Clark et al. 2009](https://pmc.ncbi.nlm.nih.gov/articles/PMC2658737)). A later study didn't replicate this ([PMC](https://pmc.ncbi.nlm.nih.gov/articles/PMC7214505)), so the evidence is mixed |
| 7 | **"Juice" and zero friction** | Every tap gives sound, motion or particles. No signup, and the game loads fast | "Juice It or Lose It" is the classic talk on this ([GDC Vault](https://gdcvault.com/play/1016487/contactUs)). Poki cut one game's load from 29.5s to 3.7s, and 72% of visitors started playing ([Poki](https://poki.com/blog/how-we-made-cannon-clash-load-fast-and-boosted-conversion)) |

**The deeper reason these work.** Players enjoy a game, and come back to it, when it makes them feel *competent* (fair challenge, clear feedback), *free* (no coercion), and *connected* (shared puzzle, comparing results) ([Ryan, Rigby & Przybylski 2006](https://link.springer.com/content/pdf/10.1007%2Fs11031-006-9051-8.pdf)). Wordle hits all three in three minutes. Its creator deliberately avoided ads and push notifications and said people like things that "transparently don't want anything from you" ([TechCrunch](https://techcrunch.com/?p=2256733)).

**Where "addictive" becomes manipulative.** Researchers catalog "dark patterns" in games, such as punishing you for missing an appointment, pay-to-skip waits, and invite-your-friends-to-progress schemes ([Zagal, Björk & Lewis 2013](https://deceptive.design/articles/dark-patterns-in-the-design-of-games)).

- **Fine:** a daily cap, streaks with a "freeze" for missed days, honest near-misses, personal bests.
- **Gray zone:** guilt-trip streak messages and nagging notifications.
- **Avoid:** faked near-misses, paid random loot, and forced accounts used to harvest data.

Forgiving streaks also help business. Letting Duolingo users bank 2 streak freezes *raised* daily users slightly ([Duolingo](https://blog.duolingo.com/duolingo-streak-research/)).

---

## How past hits spread and what they earned

| Game | Built in | How it spread | Outcome |
|---|---|---|---|
| 2048 | One weekend, by a 19-year-old | Social media, open source | 4M visitors in under a week ([City AM](https://www.cityam.com/how-one-19-year-old-won-internet-addictive-puzzler-2048/)) |
| Wordle | Side project | Emoji share grid on Twitter | Sold to NYT for "low seven figures" ([TIME](https://time.com/6143715/wordle-sale-josh-wardle-interview/)) |
| Worldle | Side project, geography reskin | Share grid | Grew into a daily-geography studio ([Teuteuf](https://teuteuf.fr/team/)) |
| Actorle | 3 days | Word of mouth | ~$4K/month two years later, self-reported ([hey.gg](https://hey.gg/blog/actorle)) |
| Rogule | Small daily roguelike | One r/WebGames post | ~2,000 daily players ([Indie Hackers](https://www.indiehackers.com/post/2000-people-per-day-are-playing-rogule-cf104c6362)) |
| Slither.io | Small team | YouTubers | ~$100K/day in ads at peak, but ~$15K/month servers ([Digital Trends](https://www.digitaltrends.com/gaming/viral-app-slither-pulls-100k-per-day/)) |
| fly.pieter.com | Built fast with AI | Creator's 600K+ X followers | Claimed $87K/month, fell to ~$12K by May 2025 ([Indie Hackers](https://www.indiehackers.com/post/2NUIOp80SUWuPmmfKoS9); [404 Media](https://404media.co/this-game-created-by-ai-vibe-coding-makes-50-000-a-month-yours-probably-wont)) |

**Lessons:**

1. **Take a known mechanic and add one twist.** Krillion is essentially Family Feud in reverse. 2048 was "a clone of a clone" ([Wikipedia](https://en.wikipedia.org/wiki/2048_(video_game))).
2. **Don't copy names or charge for free things.** Apple removed Wordle copycat apps in January 2022 after backlash ([Engadget](https://www.engadget.com/wordle-clones-app-store-232042208.html)).
3. **AI makes building cheap, but players are still the hard part.** fly.pieter.com's spike-then-drop shows this.
4. **Real-time multiplayer costs real money.** A daily puzzle served from a static page is nearly free to run.

---

## 10 original game ideas you could build

Each idea combines mechanics from above in a way that, as far as these notes show, isn't already a known hit. **Do a quick search before you start** to check for close matches. Build times assume a beginner using plain JavaScript (or Phaser for arcade games) plus an AI coding assistant.

**Difficulty key:** 🟢 Easy (a weekend to 1 week) · 🟡 Medium (1–3 weeks) · 🔴 Harder (3+ weeks)

### 1. Halfway: daily geography midpoint ⭐ recommended first build
- **Pitch:** Each day you get two cities. Tap the exact point on the map halfway between them.
- **Hook:** Shared daily puzzle, scoring by distance (mechanics 1, 4), streaks, and a share line like `Halfway #12 📍 82 km off 🔥5`.
- **Why it could spread:** Geography dailies are rising (MapTap). Results are instantly comparable ("I was 40 km off, you?"), and it works for classrooms like Krillion did.
- **Build:** 🟢 a weekend for the core, 1 week polished. Use a free map library and a list of ~500 cities, and generate each day's pair automatically, so there's no daily content to write.
- **Money:** Ads on your own domain once it has daily traffic. Optional one-time "unlimited practice" unlock, the same model reportedly used by Krillion ([dailydles](https://dailydles.com/games/krillion), unverified).

### 2. Daily Breach: spot the intruder 🔐 cybersecurity fit
- **Pitch:** Each day you get a short, fictional server log of 15–25 lines. Find the one line that shows the attacker, in as few clue-reveals as possible.
- **Hook:** A shared daily logic puzzle (logic dailies like Clues by Sam are rising), a score based on clues used, and a streak. Share line: `Daily Breach #7 🕵️ caught in 2 clues`.
- **Why it could spread:** Nothing in this space is like it. Security students, CTF players, and IT people are tight-knit communities (subreddits, Discords, school clubs), and teachers could use it in class.
- **Build:** 🟡 1–2 weeks for the engine. **The real work is writing puzzles.** Write 30 before launch. This doubles as a portfolio piece that shows you understand logs and attacks.
- **Money:** Ads are weak in this niche. Better options are sponsorship from security training companies, a paid "pack" for classrooms, or using it as a résumé project that leads to internships.

### 3. Middle Ground: guess what everyone else guesses
- **Pitch:** One estimate question a day ("How many stairs in the Eiffel Tower?"). You score by how close you are to the **crowd's median guess**, not the true answer.
- **Hook:** A crowd-scored twist in the Krillion spirit, a scale score, and a reveal chart of everyone's guesses that's fun to screenshot.
- **Why it could spread:** "What did everyone else guess?" makes people talk, and it suits group chats.
- **Build:** 🟢–🟡 1 week. It needs a tiny backend to collect guesses. **Weak spot:** with few players, the median is noisy. Show the true answer too, so the game is fun from day one.
- **Money:** Own-site ads. It's also a good fit for Reddit's platform, where Developer Funds have paid at engagement milestones (e.g., $500 at 500 daily engagers, per a 2025 thread; check current terms) ([r/Devvit mirror](https://libreddit.winscloud.net/r/Devvit/comments/1jlhi8b/the_continuation_of_reddit_developer_funds)).

### 4. Same Stack: daily tower with verified scores 🔐 cybersecurity fit (anti-cheat)
- **Pitch:** Everyone gets the same 20 oddly shaped blocks today. Stack them as high as you can. There's one attempt that counts, and unlimited practice.
- **Hook:** A daily seed, physics "juice", near-miss wobbles, and a height leaderboard.
- **Why it could spread:** Wobbling-tower clips are made for short video, and "I got 14 blocks up" is easy to compare.
- **The security angle:** Browser leaderboards are easy to cheat because players can edit scores in devtools ([Playgama](https://playgama.com/blog/business-faqs/how-to-prevent-cheating-on-client-side-leaderboards-in-html5/)). Instead of trusting the score, the game submits the player's *inputs*, and the server replays them with its own random seed to recompute the score. This is the approach used by Open Hexagon and others ([GIGAZINE](https://gigazine.net/gsc_news/en/20211110-open-hexagon-against-cheet); [DEV](https://dev.to/gowtham_r_2002/dont-trust-the-score-building-server-authoritative-validation-for-a-prize-based-mobile-game-246i)). A write-up of this ("I threat-modeled my own game") is a strong portfolio piece.
- **Build:** 🟡–🔴 2–4 weeks. Physics replay that matches exactly is genuinely tricky. Ship without the leaderboard first.
- **Money:** Poki or CrazyGames revenue share. Poki reportedly gives you 100% of earnings from players you bring in yourself and 50% from players it sends ([Poki SDK](https://sdk.poki.com/deals), search summary).

### 5. One Pixel Short: one-button precision arcade
- **Pitch:** A circle grows. Tap to stop it exactly filling a gap. Each level the gap gets weirder.
- **Hook:** Restart in under a second, a "98.7% — so close!" readout (mechanic 6), heavy juice, and a personal best always on screen.
- **Why it could spread:** You learn it in one second. It suits portals and phones, and the near-miss percentages make good screenshots.
- **Build:** 🟢 a weekend for a playable version, 1 week polished. This is the smallest idea on the list.
- **Money:** Poki/CrazyGames ads. CrazyGames' top games load in under 10 seconds and are under 20 MB ([CrazyGames docs](https://docs.crazygames.com/resources/basic-launch-metrics/)), which is easy for a game this small.

### 6. First Finder: word chain where firsts are forever
- **Pitch:** Today's starting word is "OCEAN". Chain related words, e.g., OCEAN → TIDE → MOON. Any link that no one has ever played before is credited to you permanently.
- **Hook:** Brag-worthy "firsts" like Infinite Craft (mechanic 5), a daily start word, and a profile of your discoveries.
- **Why it could spread:** "I discovered 3 links nobody had ever found" invites screenshots.
- **Build:** 🟡 2–3 weeks. You need a way to judge whether two words are related, such as a word-association dataset. Avoid an AI model judging links, because costs add up and players are suspicious of AI-judged answers (Krillion's creator faced questions about AI use).
- **Money:** Own-site ads, plus a one-time unlock for an archive of past days.

### 7. Rank Order: sort it blind
- **Pitch:** Six items (e.g., animals) to sort by a hidden property (e.g., top speed). After each try you're told only *how many* are in the right spot, like the board game Mastermind.
- **Hook:** A daily puzzle, a limited number of tries, and a share grid of your attempts.
- **Why it could spread:** Easy to theme for any fandom (Pokémon stats, movie box office, game release dates), the same reskin trick that made Worldle and Heardle work.
- **Build:** 🟢 1 week. Content is a list of 6 items per day, and spreadsheet data makes that easy. Check first for existing "sort it" dailies, since this space may be crowded.
- **Money:** Ads, or launch versions for specific fandoms as separate sites (a small "studio" approach, like Teuteuf).

### 8. Night Lights: a city lit by today's players
- **Pitch:** One shared night-time city. Solve today's 60-second mini-puzzle and you light one window. By midnight, the city shows everyone who played.
- **Hook:** Relatedness and cozy shared presence (like Messenger and One Million Checkboxes), with a daily cap.
- **Why it could spread:** "Look, I'm that window" is a calm, beautiful thing to share, and it fits the trend away from AI-generated content.
- **Build:** 🟡–🔴 3+ weeks. It needs live shared state. Cloudflare's free tier now covers this, but caps you at 100K requests a day ([Cloudflare](https://developers.cloudflare.com/workers/platform/pricing/)).
- **Money:** Tips/Patreon or sponsorships. Ads would spoil the mood.

### 9. Human or Bot?: spot the real person
- **Pitch:** You see six short answers to yesterday's prompt. Some were written by players and some were generated. Pick the humans. Tomorrow, your answer joins the pool.
- **Hook:** A daily loop where players create the content, a scale score, and an anti-AI cultural moment (Your AI Slop Bores Me went viral on this mood).
- **Why it could spread:** People love arguing about what "sounds like AI".
- **Build:** 🟡 2–3 weeks. **Weak spot:** you must filter what players submit before showing it to others. That's moderation work, and bad content can get your ads account banned. One developer reported surviving an AdSense ban ([DEV](https://dev.to/yitao/post-mortem-how-my-web-game-hit-130k-mau-with-0-marketing-and-survived-an-adsense-ban-883)). There's also a light security angle, since this is bot detection.
- **Money:** Ads and a Reddit version.

### 10. Low Tide: a 20-minute incremental with an ending
- **Pitch:** Build a sandcastle kingdom before the tide comes in. Numbers go up and upgrades multiply. It ends in about 20 minutes with a shareable finish time.
- **Hook:** The incremental "numbers go up" loop, where costs rise about 1.15x per purchase as in Cookie Clicker ([arXiv](https://arxiv.org/pdf/1808.07540)), but with a *real ending*, so it respects players' time.
- **Why it could spread:** r/incremental_games is an active audience, and "beat it in 17:42" invites speedruns.
- **Build:** 🟡 2–3 weeks. Balancing the numbers takes longer than coding them.
- **Money:** A free web version plus a paid mobile or Steam port. This is a proven path: A Dark Room's iOS port grossed about $697K over two years ([Game Developer](https://gamedeveloper.com/business/a-two-year-look-at-the-sales-of-chart-topping-ios-title-i-a-dark-room-i-)), and Universal Paperclips sells a $1.99 app ([App Store](https://apps.apple.com/us/app/id1300634274)).

### All ideas at a glance

| Idea | Type | Difficulty | Time (solo beginner) | Daily content work? | Best money path |
|---|---|---|---|---|---|
| 1. Halfway ⭐ | Daily geography | 🟢 | Weekend–1 wk | None (auto-generated) | Own-site ads, unlock |
| 2. Daily Breach 🔐 | Daily logic | 🟡 | 1–2 wks + puzzles | High | Sponsorship, portfolio |
| 3. Middle Ground | Daily crowd trivia | 🟢–🟡 | ~1 wk | Low (1 question/day) | Ads, Reddit funds |
| 4. Same Stack 🔐 | Daily physics | 🟡–🔴 | 2–4 wks | None (seeded) | Portals |
| 5. One Pixel Short | Arcade | 🟢 | Weekend–1 wk | None | Portals |
| 6. First Finder | Daily word | 🟡 | 2–3 wks | Low | Ads, unlock |
| 7. Rank Order | Daily trivia | 🟢 | ~1 wk | Medium | Ads, fandom spin-offs |
| 8. Night Lights | Cozy multiplayer | 🟡–🔴 | 3+ wks | Low | Tips, sponsors |
| 9. Human or Bot? | Daily social | 🟡 | 2–3 wks | Players create it | Ads, Reddit |
| 10. Low Tide | Incremental | 🟡 | 2–3 wks | None | Paid port |

### Honest money expectations

- **Most indie web games earn little.** The realistic first dollars come from a portal revenue share, a Reddit Devvit program, or ads on a daily game that people return to.
- **Self-reported success stories** sit in the few-thousand-dollars-a-month range: Actorle at ~$4K/month ([hey.gg](https://hey.gg/blog/actorle)) and a solitaire site at $10K/month ([Indie Hackers](https://www.indiehackers.com/post/how-i-grew-a-simple-solitaire-game-to-10k-mrr-28e352c308)).
- **Acquisitions like Wordle's are rare outliers.** Even Heardle, bought by Spotify, was shut down about nine months later ([Wikipedia](https://wikipedia.com/wiki/Heardle)).
- **If you run ads on your own site, check your host's terms.** Vercel's free Hobby plan reportedly bans commercial use (not re-verified for 2026). Cloudflare Pages or GitHub Pages are safer choices.

---

## 10 more ideas: survival, boss fights, snow and golf

These ideas use the same seven mechanics, applied to the four themes you suggested. The same rule applies: **search for close matches before you build.** Daily golf games and community "world boss" events already exist, so the twist is what makes each one yours.

### 11. Daily Descent: one mountain, everyone skis it ⛷️
- **Pitch:** Each day the game generates one ski course, and the whole world races the same run. Steering is left/right only.
- **Hook:** Shared daily puzzle (1), score on a scale (4), and "one more try" (6). You get 3 runs a day and the best one counts. You race the ghost of the median player, so you always have a rival who is about as good as you.
- **Why it could spread:** Times are easy to compare ("41.2s, beat me"). Share line: `Descent #8 ⛷️ 41.2s · top 18% 🔥4`.
- **Build:** 🟡 1–2 weeks with Phaser. The course comes from a date-based seed, so there's no content to write. Ghosts are just lists of saved positions.
- **Money:** Portal version with unlimited random mountains. Keep the daily mountain on your own site.

### 12. Outrun: snowboard ahead of the avalanche 🏂
- **Pitch:** An endless downhill game with an avalanche chasing you. Tricks off jumps give speed. A trick you don't land costs speed, and the snow gets closer.
- **Hook:** "One more try" (6) with constant near-misses, because the avalanche is always on screen. Juice (7) from powder spray, screen shake and the rumble getting louder. Risk and reward: a bigger trick means more speed but a higher chance of crashing.
- **Why it could spread:** Escaping the avalanche by a pixel makes a great short clip for TikTok or YouTube Shorts.
- **Build:** 🟢–🟡 1 week. One-button tricks: hold to spin, release to land.
- **Money:** Built for Poki and CrazyGames (the portal revenue share). Unlockable boards and outfits make a natural rewarded-ad slot.

### 13. Crowd Green: today's hole was shaped by yesterday's players ⛳
- **Pitch:** One golf hole a day. Overnight, the most popular landing spot from yesterday's players becomes a sand trap on today's course.
- **Hook:** Shared puzzle (1) plus a crowd twist. Yesterday's players literally shape today's course, so the "safe" shot keeps changing. Score vs. par (4). Share line: `Crowd Green #21 ⛳ -1 (birdie) 🟩🟩🟨`.
- **Why it could spread:** Every hole comes with a story ("everyone hit left yesterday, so left is a bunker now"), which gives people something to talk about.
- **Build:** 🟡 1–2 weeks. Top-down 2D golf, plus a small server that counts landing spots and places tomorrow's hazards.
- **Money:** Ads on your own site. A golf brand or local course is also a plausible sponsor.

### 14. One Putt: a daily bank-shot puzzle ⛳ ⭐ easiest of this batch
- **Pitch:** One strange mini-golf green a day: walls, bumpers and portals. Find the single shot that sinks it. Unlimited attempts, and your score is how many you needed.
- **Hook:** Wordle's structure (fewest tries wins) on a physics puzzle (1, 2, 3). Every miss shows you something, so "so close" feels fair (6).
- **Why it could spread:** "Got it in 2" invites "no way, I needed 9." Share line: `One Putt #30 ⛳ 3 tries 🔥12`.
- **Build:** 🟢 a weekend. A ball bouncing off straight walls is simple math, so you don't need a physics engine. Making greens is fun, and a few can be generated by code.
- **Money:** Ads plus a one-time "course pack" of past greens, the same archive-unlock model reportedly used by Krillion.

### 15. World Boss: everyone fights the same boss today 🐉
- **Pitch:** One boss a day with a big shared health bar. Each player gets 3 attempts, and the damage you deal comes off the global bar. If the world kills it by midnight, everyone who helped earns that day's trophy.
- **Hook:** Connection (feeling part of something bigger, from the "deeper reason" research) plus the shared daily event (1). Rare moments (5): "top damage today" and "landed the killing blow."
- **Why it could spread:** "The boss is at 4% HP with 2 hours left" makes people pull in their friends. It's a natural fit for Reddit Devvit or Discord Activities.
- **Build:** 🟡–🔴 2–4 weeks. Simple action combat plus a server counter. 🔐 **Cybersecurity fit:** a shared HP bar is an obvious target for cheaters, so verify damage by replaying moves on the server (the same anti-cheat idea as Same Stack).
- **Money:** Reddit developer funds and Discord. Cosmetic trophies.

### 16. Rare Build: beat the boss with a loadout nobody else picked 🃏
- **Pitch:** Before each daily boss fight, you draft 3 abilities from 8. Winning counts, but your score is based on how rare your winning build was, Krillion-style.
- **Hook:** Rarity scoring (4, 5) moved into a boss fight. Winning with the obvious build scores 20. Winning with a build only 0.3% of players tried earns "One in a Thousand."
- **Why it could spread:** It's the Krillion format, which is trending right now, applied to a new genre. People share strange builds that somehow won.
- **Build:** 🟡 2 weeks. Turn-based fights are much easier than action combat, and the server only needs to count which builds people picked.
- **Money:** Ads. A good candidate for a paid "endless mode" later.

### 17. Last Light: survive seven nights in five minutes 🔥
- **Pitch:** A survival game played with cards. Each night you choose: gather wood, find food, fortify, or explore. Each choice risks something. Get through 7 nights. Everyone plays the same daily seed.
- **Hook:** Daily shared run (1), short and replayable, plus a clean share line: `Last Light #9 🌑🌑🌑🌑🌑🔥🔥 survived 7/7`. The near-miss of dying on night 6 gives you "one more try."
- **Why it could spread:** Comparing "how did you survive night 4?" leads to strategy talk, which is free word of mouth.
- **Build:** 🟢 about 1 week. Mostly text and choices with simple art. No physics, no real-time action. Great for staying focused.
- **Money:** Ads, plus an "endless" random-seed mode as a one-time unlock.

### 18. The Colony: survive together, one vote a day 🏕️
- **Pitch:** One shared group of survivors for all players. Each day everyone votes on the colony's next move: ration food, scout the ruins, take in strangers. Tomorrow the results play out, and the story continues for weeks.
- **Hook:** Connection (feeling part of something) plus a daily appointment, without punishing people who miss a day. "Day 47 of the colony" gives people a reason to come back that doesn't depend on streak pressure.
- **Why it could spread:** Built for Reddit Devvit. Each day's result can be its own post, and the comment arguments are the marketing.
- **Build:** 🟡 2–3 weeks, plus a few minutes of writing each day. AI can help draft event text, but you edit it.
- **Money:** Reddit developer funds (they pay by daily player count). A "Season 1" archive.

### 19. Uptime: keep the server alive 🖥️ 🔐 cybersecurity fit
- **Pitch:** A survival game where you're the night-shift sysadmin. Alerts pour in, such as failed logins, a CPU spike or an odd outbound connection, and you triage each one: block, patch, ignore or escalate. Survive until 6 a.m. without a breach.
- **Hook:** Survival pressure (one more shift), escalating difficulty, a score for minutes of uptime, plus a daily seed so everyone gets the same night. Share line: `Uptime #5 🟢🟢🟢🟡🔴 breached at 4:12 a.m.`
- **Why it could spread:** Security and IT communities (r/sysadmin, r/cybersecurity) love games about their jobs, and it's a great portfolio piece that shows you know what real alerts look like.
- **Build:** 🟡 2 weeks. A user interface with timers, no game engine needed. The real work is writing realistic alerts, which is also good study.
- **Money:** Sponsorship from security training companies is plausible. Mainly a portfolio and résumé piece.

### 20. Patch the Boss: win by finding its bug 🐛 🔐 cybersecurity fit
- **Pitch:** A boss fight you can't win by attacking. Each boss has a flaw, like taking a negative number for damage, never checking whether you're really an "admin," or a timing gap during its windup. Find the flaw and exploit it.
- **Hook:** A puzzle in boss form. The "aha" moment is a rare moment you want to brag about (5). A daily boss with a shared flaw gives a share line like `Patch the Boss #3 🐛 found in 4 tries`.
- **Why it could spread:** Players learn real ideas, such as input validation, broken access control and race conditions, without it feeling like class. Capture-the-flag (CTF) players and teachers would share it.
- **Build:** 🟡 2–3 weeks. Each boss is a small puzzle with a deliberate bug. Make sure the only bugs are the ones you meant to include.
- **Money:** Portfolio and teaching use first. School licenses or sponsorship later.

### The second batch at a glance

| Idea | Theme | Difficulty | Time | Best money path |
|---|---|---|---|---|
| 11. Daily Descent | Skiing | 🟡 | 1–2 wks | Own site + portal spin-off |
| 12. Outrun | Snowboarding + survival | 🟢–🟡 | ~1 wk | Portals |
| 13. Crowd Green | Golf | 🟡 | 1–2 wks | Ads, sponsor |
| 14. One Putt ⭐ | Golf | 🟢 | Weekend | Ads, unlock |
| 15. World Boss 🔐 | Boss fight | 🟡–🔴 | 2–4 wks | Reddit, Discord |
| 16. Rare Build | Boss fight | 🟡 | ~2 wks | Ads, unlock |
| 17. Last Light | Survival | 🟢 | ~1 wk | Ads, unlock |
| 18. The Colony | Survival | 🟡 | 2–3 wks | Reddit funds |
| 19. Uptime 🔐 | Survival + security | 🟡 | ~2 wks | Portfolio, sponsor |
| 20. Patch the Boss 🔐 | Boss + security | 🟡 | 2–3 wks | Portfolio, teaching |

**If you only build one from this batch:** start with **One Putt** (a weekend) or **Last Light** (about a week). Both are small enough to finish and have a share line that's easy to copy. **Outrun** is the best bet for portal money, and **Uptime** or **Patch the Boss** is the best for your résumé.

---


## Start here: ship Halfway in about two weeks

Long projects are the enemy, so the plan is built around **tiny finish lines**. Each step ends with something playable.

| When | Goal | Done when… |
|---|---|---|
| **Day 1** (3–4 hrs) | Map on screen; two city names; you tap and see the distance | You can play one round, even if it's ugly |
| **Day 2** | Same pair for everyone today, chosen from the date and a city list; score 0–100 | Two friends get the same puzzle |
| **Day 3** | Share button that copies `Halfway #3 📍 82 km 🔥2` (no answer, no spoiler) | You've pasted it into a group chat |
| **Day 4** | Streak + stats saved in the browser (no accounts); streak freeze after 7 days | Refreshing the page keeps your streak |
| **Days 5–6** | Juice: a pin-drop animation, a line drawn to the true midpoint, a sound | It feels satisfying on your phone |
| **Week 2** | **Security pass:** move the answer to a tiny Cloudflare Worker so it isn't sitting in the page code (Wordle shipped every future answer in its JavaScript ([PCWorld](https://www.pcworld.com/article/606109/how-to-cheat-at-wordle.html))); add rate limits | Viewing the page source doesn't reveal tomorrow's answer |
| **Launch** | Free hosting on Cloudflare Pages ([free tier](https://developers.cloudflare.com/workers/platform/pricing/)) with a short, memorable domain | Live URL |

**Launch checklist:**

1. Share it with friends, a class group chat, and a geography teacher.
2. Post once to r/WebGames, following its rules. One good post there grew Rogule to ~2,000 daily players ([Indie Hackers](https://www.indiehackers.com/post/2000-people-per-day-are-playing-rogule-cf104c6362)). Spamming five subreddits at once flopped for another developer ([Indie Hackers](https://www.indiehackers.com/post/i-posted-my-browser-moba-shooter-to-5-subreddits-and-got-3-upvotes-then-i-gave-it-a-map-editor-8038535a59)).
3. Ask daily-game aggregators like Playlin and dlegames whether they list new games.
4. Write a short blog post: "How I stopped players from reading tomorrow's answer". It's your portfolio piece.

**Rules to keep yourself finishing:**

- **Freeze the feature list** at what's in the table. New ideas go in a "v2" note, not the code.
- **Ship ugly on Day 1.** A playable bad version beats a perfect plan.
- **Timebox:** if Halfway isn't live in three weeks, cut features until it is.
- **Then decide with data.** If people return for a week, add ads and a practice-mode unlock. If they don't, move on to idea #2 (Daily Breach) or #5 (One Pixel Short). Your code for daily seeds, sharing and streaks carries over to every daily idea on this list.

---

## Conclusion

The pattern behind 2026's hits isn't new technology. It's restraint: one shared puzzle, a few minutes, a score worth comparing, and a result people *want* to paste into a group chat. That suits a solo student well, because the hard parts are good design and getting players, not engineering. Your security background is a real edge in a niche that mostly ignores it. Most daily games still leak answers or accept fake scores, so "built properly" is both a selling point and a résumé line. Treat the first game as a reusable kit (daily seed, share text, streaks, server-checked answers) rather than a one-shot bet. Each later idea then costs days, not weeks, and having several small games is how solo developers like Teuteuf and neal.fun turned one hit into steady traffic.

*Sourcing note: the underlying research could not open most pages directly and relied on search-result summaries. Figures marked self-reported, secondary, or unverified, and everything about Krillion's creator, launch and player numbers, should be double-checked before you rely on them.*
