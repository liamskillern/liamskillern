# Design Principles and Psychology Behind Compulsively Replayable Casual Browser Games

> Method note: This session could not fetch full pages (wikipedia.org, gamedeveloper.com and others failed DNS resolution under the session's network allowlist). All findings below come from web search result summaries and snippets, so quotes and numbers should be spot-checked against the linked pages before publication. Where search snippets disagreed, this is noted.

## 1. Daily return and habit formation (daily limits, streaks, shared global puzzle, countdown, habit loops)

### Takeaway
The strongest evidence for daily return comes from Wordle/NYT Games (one shared puzzle per day, streak stats) and Duolingo's published streak experiments. Scarcity (one puzzle a day) plus a shared puzzle plus streaks turns a 3-minute game into a daily ritual that has lasted for years: Wordle was played billions of times a year from 2023 to 2025.

### Cited Findings
- Wordle's 2013 prototype had **infinite play**, meaning players could immediately start another round. The once-per-day limit came with the 2021 version. — [PocketGamer.biz on Wardle's GDC talk](https://www.pocketgamer.biz/news/78481/gdc-josh-wardle-shares-his-incorrect-tips-for-wordles-success/)
- Wardle's GDC 2022 talk was titled "Wordle: Doing the Opposite of What You're Meant To" (Design track). — [GDC Vault](https://www.gdcvault.com/play/1027882/css/home.css)
- Wardle cited daily games such as the NYT Crossword and Spelling Bee as inspiration. — [Android Central](https://www.androidcentral.com/apps-software/josh-wardle-tried-to-make-wordle-android-app-2013)
- Wardle said the game "encourages you to spend three minutes a day" and doesn't want more of your time than that. He also said he was "suspicious of mobile apps that demand your attention and send you push notifications." — [DT Next via PressReader](https://pressreader.com/india/dt-next/20220105/281998970800660); [TechCrunch](https://techcrunch.com/?p=2256733)
- SNHU psychologist Josh Garrin ties the one-game-a-day format to the **scarcity principle**. — [SNHU](https://www.snhu.edu/about-us/newsroom/hot-topics/psychology-of-wordle)
- Social psychologist Matthew Baldwin argues that Wordle differs from Sudoku or Words With Friends because everyone shares a **common goal**: the same puzzle on the same day. — [Science Friday / related coverage](https://www.sciencefriday.com/segments/why-we-love-wordle/) (attribution from search summary; verify)
- Long-run scale of the daily ritual: Wordle was played 4.8B times in 2023 ([Axios](https://www.axios.com/2024/01/29/wordle-nyt-games-news-media-layoffs)), 5.3B in 2024 ([CBS News](https://www.cbsnews.com/news/wordle-the-daily-obsessions-of-millions); [TODAY via AOL](https://www.aol.com/exclusive-wordle-puzzle-ended-5-013624721.html)), and 4.2B solved in 2025 ([NBC](https://www.nbcnewyork.com/entertainment/entertainment-news/hardest-wordle-connections-games-2025/6436464/)). Note that the 2025 figure is "solved", not "played", so the decline may partly reflect a different metric.
- NYT Games puzzles in 2024: 11.1B solved in total, including Mini 2.1B and Strands 1.3B. — [TODAY via AOL](https://www.aol.com/exclusive-wordle-puzzle-ended-5-013624721.html). In 2025, Connections had 1.6B solves, Strands 1.5B, Mini 1.4B, Spelling Bee 667M and Pips 612M. — [NBC New York](https://www.nbcnewyork.com/entertainment/entertainment-news/hardest-wordle-connections-games-2025/6436464/)
- Streaks are a big enough deal that NYT reports streak breaks as news. On Oct 15, 2024, the word "CORER" ended **5.6 million streaks** ([TODAY via AOL](https://www.aol.com/exclusive-wordle-puzzle-ended-5-013624721.html)). "BONGO" snapped 36,337 streaks ([NBC](https://www.nbcnewyork.com/entertainment/entertainment-news/hardest-wordle-connections-games-2025/6436464/)).
- Duolingo (first-party data): learners who reach a **7-day streak are 2.4x more likely** to come back the next day. — [Duolingo blog](https://blog.duolingo.com/how-duolingo-streak-builds-habit)
- Duolingo's "Streak Wager" A/B test produced significant gains in D1, D7 and D14 retention, with **D7 up 14%**. — [Duolingo blog](https://blog.duolingo.com/improving-the-streak)
- Raising the Streak Freeze limit to 2 increased daily active learners by **0.38%** and did not cause the feared drop-off from people skipping lessons. — [Duolingo streak research](https://blog.duolingo.com/duolingo-streak-research/) (Japanese-language post, summarized)
- Separating two streak mechanics increased D14 retention by 3.3% and overall DAU by 1%. — [Duolingo engineering blog](https://making.duolingo.com/how-streaks-keep-duolingo-learners-committed-to-their-language-goals)
- The Hooked model (Nir Eyal, 2014) has four phases: **trigger → action → variable reward → investment**. — [Medium / Behavior Design](https://medium.com/behavior-design/hooked-on-loot-boxes-how-design-gets-us-addicted-79c45faebc05)
- A business-school analysis argues NYT bought Wordle for attention, habit and daily engagement, and uses it as a gateway into the wider NYT Games bundle (Connections, Strands and others follow the same quick, shareable daily format). This is opinion, not metrics. — [Ivey Business School](https://ivey.uwo.ca/hba/blog/2025/03/the-daily-puzzle-phenomenon-how-nyt-turned-games-into-a-subscription-goldmine)

### Inferences
- Wordle's Hooked loop maps as follows. **Trigger:** external at first (friends' grids on social feeds), then internal (morning coffee, or "a new puzzle is out"). **Action:** at most 6 guesses. **Variable reward:** solved in 2 vs. 6 tries, plus the tile-flip reveal. **Investment:** the streak and the guess-distribution histogram, which you lose by skipping a day.
- The daily cap does two jobs. It creates scarcity ("leave them wanting more"), and it lets the puzzle be shared globally, which in turn makes comparison and conversation possible. A solo developer should treat "one seeded puzzle per day for everyone, same puzzle number" as a single design unit.
- Countdown-to-next-puzzle timers are standard in Wordle-likes, but no source here measured their effect. Treat them as conventional, not proven.
- Streak forgiveness, such as freezes or repair, appears to help retention (Duolingo data). It also lowers the anxiety and punishment side of streaks; see section 6.
- The NYT has built a portfolio (Wordle → Connections → Strands → Pips) around the same template. This suggests the format generalizes beyond words: daily + short + shared + streak.

### Gaps
- No peer-reviewed study isolating the effect of the "one per day" limit on Wordle retention was found. The claims are expert commentary from 2022 (Tufts, SNHU, Calgary, Psychology Today).
- No NYT-published DAU or retention curve was found. NYT reports annual plays only.
- No data was found on the effect of countdown timers.
- Habit-formation research (e.g., Lally et al. on how long habits take to form) was not retrieved in this session.

## 2. Shareability and virality (emoji grid, spoiler-free sharing, social comparison, Wordle's growth numbers)

### Takeaway
Wordle's growth curve is the canonical case: about 90 players at the start of November 2021, 300,000 around Jan 2, 2022, and 2M+ a week later. The spike followed the December 2021 addition of the copy-to-clipboard emoji grid. A player invented that grid, not Wardle. It was spoiler-free and visually recognizable, and it worked as status-signalling content that made others curious enough to search for the game.

### Cited Findings
- Growth: **90 players on Nov 1, 2021 → 300,000 on Jan 2, 2022 → more than 2 million a week later.** — [Statista](https://www.statista.com/chart/amp/26667/usage-of-wordle-and-other-online-games-in-the-us); [World Economic Forum](https://www.weforum.org/stories/all/wordle-game-new-york-times-business-plan/). Caveat: some secondary sources date the 300k milestone to late December 2021, and most numbers are estimates rather than disclosed figures ([levvvel](https://levvvel.com/wordle-statistics/); [fictionhorizon](https://fictionhorizon.com/how-many-people-play-wordle/)).
- The game took off in **December 2021 after Wardle added the ability to copy results as emoji squares**, which were widely shared on Twitter. — [Wikipedia (via search)](https://en.wikipedia.org/wiki/Wordle); [NPR](https://www.npr.org/2022/01/14/1072980440/a-simple-word-game-is-the-newest-social-media-phenomenon)
- The emoji-grid idea came from **an early player in New Zealand** (Elizabeth S), who began posting results as emoji. Wardle then built it into the game. — [Know Your Meme](https://knowyourmeme.com/memes/subcultures/wordle); [Wikipedia](https://en.wikipedia.org/wiki/Wordle)
- The share text **contained no URL**, so growth came from curious people searching for the game. — [Know Your Meme / Wikipedia via search summary](https://knowyourmeme.com/memes/subcultures/wordle)
- Psychology Today suggests instant performance feedback and the option to post results on social media are central to Wordle's success. — [Psychology Today](https://psychologytoday.com/nz/blog/the-asymmetric-brain/202201/the-psychology-behind-wordle)
- Tufts psychologist Holly Taylor attributes the appeal to "desirable difficulty": success isn't guaranteed. — [Tufts Now](https://now.tufts.edu/2022/01/27/what-our-brains-do-when-we-play-wordle)
- Calgary psychologist Penny Pexman says Wordle offers "a daily dose of complex cognition combined with social interaction". She does not claim it makes you smarter. — [University of Calgary](https://ucalgary.ca/news/wordle-craze-why-do-we-love-puzzles-and-are-they-good-our-brains-0)
- The NYT bought Wordle on Jan 31, 2022 for a "low seven-figure sum". — [AdRoll summary](https://www.adroll.com/blog/unrolling-wordle-how-a-pet-project-sold-for-7-figures); [TechCrunch](https://techcrunch.com/2022/05/04/wordle-new-york-times-user-growth). Wordle reportedly brought "tens of millions" of new users to the NYT. — [AOL/Engadget](https://www.aol.com/news/wordle-brought-tens-millions-users-150000203.html)
- Infinite Craft (Neal Agarwal, released Jan 31, 2024) is a 2024 viral example. Its "**First Discovery**" mechanic credits you if you are the first person ever to craft an item, which creates bragging-rights screenshots. Two days after launch, players were crafting nearly **1,000 items per second**, and Agarwal said "It's been a struggle keeping the servers up". — [Wikipedia (via search)](https://en.wikipedia.org/wiki/Infinite_Craft); [Destructoid](https://destructoid.com/?p=460007); [PC Gamer](https://www.pcgamer.com/this-browser-based-endless-crafting-game-starts-you-off-with-fire-and-water-but-it-quickly-escalates-to-god-the-big-bang-and-yin-yoda). No verified total player count was found.

### Inferences
Checklist for a shareable result:
- **Spoiler-free:** it shows how you did, not the answer.
- **Unique per player:** each grid looks different, which invites comparison.
- **Comparable:** everyone played the same puzzle, and the puzzle number gives context.
- **Compact and copyable plain text:** emoji works in every chat app, with no image upload.
- **Mysterious to outsiders:** colored squares make people ask "what is this?"
- The no-URL choice probably made sharing feel less like advertising and more like social expression. A developer today might include a short URL, but keep the grid as the hero. This is a tradeoff, untested.
- Players created the grid behavior first. Watch what players already do (screenshots, copy-paste) and productize it.
- "Firsts" and rare outcomes (Infinite Craft first discoveries, a 1/6 Wordle) are inherently braggable. Design for rare, screenshot-worthy moments.

### Gaps
- Wardle's GDC talk content on why he chose the share format was not accessible (GDC Vault paywall / fetch blocked).
- No quantitative viral coefficient (K-factor) for Wordle was found.
- No academic study on emoji-grid sharing as a growth mechanic was found.

## 3. "One more try" in session-based games (short sessions, fast restart, near-misses, variable rewards, mastery, flow, juice, incremental progression)

### Takeaway
"One more try" draws on several distinct levers. Near-misses raise the desire to keep playing (Clark 2009, gambling context, with mixed replication). Variable rewards produce persistent behavior. Flow comes from keeping challenge matched to skill (Csikszentmihalyi, Jenova Chen's *flOw*). "Juice" is abundant feedback on every input (Jonasson & Purho, 2012). Incremental games keep numbers going up through exponential cost scaling (Cookie Clicker uses a ×1.15 cost multiplier).

### Cited Findings
- Near-misses: Clark et al. (2009, *Neuron*) found near-misses were rated **less pleasant** than full misses, yet **increased the desire to play**, and recruited win-related brain circuitry. The effect was stronger when players had **personal control**. — [Clark et al. 2009, PMC](https://pmc.ncbi.nlm.nih.gov/articles/PMC2658737)
- Counter-evidence: a 2020 study in pigeons and humans "failed to support the near-miss effect hypothesis". — [PMC7214505](https://pmc.ncbi.nlm.nih.gov/articles/PMC7214505)
- Variable ratio reinforcement: random reward mechanisms such as loot boxes are variable-ratio schedules, "known to produce highly persistent behaviors". — [Kao, MIT](https://people.csail.mit.edu/dkao/pdf/kao2019tog.pdf); [Australian Senate inquiry](https://aph.gov.au/Parliamentary_Business/Committees/Senate/Environment_and_Communications/Gamingmicro-transactions/Report/c03)
- Rare loot-box rewards produce larger arousal and reward responses and a greater urge to open more. — [Larche et al. 2019 via search summary, Springer](https://link.springer.com/article/10.1007%2Fs10899-019-09891-8)
- Flow and dynamic difficulty: Jenova Chen's USC thesis on dynamic difficulty adjustment produced *flOw*. Chen used "User-Centered DDA", where players choose difficulty implicitly (diving between planes, choosing which creatures to eat) rather than the game silently tuning it. The approach rests on Csikszentmihalyi's balance between ability level and challenge. — [Wikipedia: Flow (video game)](https://en.wikipedia.org/wiki/Flow_(video_game)); [Engadget 2006](https://www.engadget.com/2006-09-12-flow-in-games-an-interactive-thesis-on-dynamic-difficulty.html); [Medium: Exploring Systems: Flow](https://medium.com/serious-games-377g/exploring-systems-flow-88672b3dd21f)
- Critique: some argue flow can occur without difficulty, as in The Sims. — [Medium](https://medium.com/serious-games-377g/exploring-systems-flow-88672b3dd21f)
- Juice: in "Juice It or Lose It" (GDC/Nordic Game 2012), Martin Jonasson and Petri Purho add particles, screenshake, sound and animation step by step to a plain breakout clone. They define juice as "abundant feedback" on interaction. — [GDC Vault](https://gdcvault.com/play/1016487/contactUs); [roblog](https://roblog.co.uk/2024/03/juicy-games/)
- Caveat: "not all juice is good juice". Better game feel comes from moderation and context. Folmer Kelly argued at GDC Europe that over-polish can reduce immersion. — [arXiv 2011.09201 (Pichlmair & Johansen survey)](https://arxiv.org/abs/2011.09201)
- Game feel is "the intentional design of the affective impact of moment-to-moment interaction". Swink's *Game Feel* plus the Jonasson/Purho and Nijman talks remain the primary sources. — [arXiv 2011.09201](https://arxiv.org/abs/2011.09201)
- Incremental/idle: Cookie Clicker (Orteil, 2013) starts with one cookie per click, and building costs rise by a factor of **1.15 per purchase**, with exponential late-game scaling. — [arXiv 1808.07540](https://arxiv.org/pdf/1808.07540); [Wikipedia](https://en.wikipedia.org/wiki/Cookie_Clicker)
- Cookie Clicker descends from parodies (Progress Quest, Cow Clicker) meant to show how hollow progress mechanics are. Cow Clicker "inadvertently showed the opposite". Sebastian Deterding calls Cookie Clicker a "perfect exemplar" of gamification, where progress mechanics make rote clicking compelling. — [Deterding, White Rose eprints](https://eprints.whiterose.ac.uk/146788/1/25_Deterding_draft_final_180515_SDE.pdf)
- Idle games are defined as games that "progress with minimal or no player interaction". — [Alharthi et al., NSF PAR](https://par.nsf.gov/servlets/purl/10061230)
- "Desirable difficulty": Wordle's success isn't guaranteed. — [Tufts Now](https://now.tufts.edu/2022/01/27/what-our-brains-do-when-we-play-wordle)

### Inferences
"One more try" checklist:
- Restart in under 1 second, with no menu between death and retry.
- Runs short enough that a failure costs little.
- Make failure visibly *close*, e.g., a "you were 3% away" progress bar or a best-score ghost. Near-misses work best when the player feels in control.
- Keep a personal best always visible.
- Put juice on every input (sound, squash and stretch, particles, screenshake), in moderation.
- Ramp difficulty, or let players self-select it.
- For idle and incremental games, use exponential costs (about ×1.07–1.15) against multiplicative upgrades so a new goal is always just in reach. Prestige/reset layers extend this.
- Near-miss engineering borrowed from gambling is the most ethically loaded lever (see section 6). Near-misses that arise from real skill (a platformer death a pixel short) differ from faked near-misses (rigged reels).

### Gaps
- No full text was retrieved for Swink's book or Koster's *A Theory of Fun*. Koster's thesis ("fun is learning / pattern mastery"; boredom once a pattern is mastered) is well known but was not sourced in this session.
- No empirical data on restart speed vs. retention for browser games was found.
- Csikszentmihalyi's primary text and Chen's 2007 CACM "Flow in Games" paper were not retrieved directly.

## 4. Low friction (no signup, no download, instant load, mobile-friendly, simple rules)

### Takeaway
Browser portals publish hard data showing load time and build size drive "conversion to play". Poki's Stickman Hook case went from a 29.5s median load to 3.7s, and conversion to play rose to 72%. CrazyGames' top titles load in under 10s, ship builds under 20 MB, and convert 80%+. Wordle and neal.fun pair zero friction (web, no account, no ads) with simple rules.

### Cited Findings
- Poki case: Stickman Hook's WebGL port was 40 MB with a **29.5s median load**. An HTML5 rebuild at 6 MB brought the median load to **3.7s**, and **conversion to play rose to 72%**. — [Poki blog](https://poki.com/blog/how-we-made-cannon-clash-load-fast-and-boosted-conversion) (vendor-reported, single example; the result appeared under this URL in search, which may be a related post)
- CrazyGames: top-performing titles "typically convert 80%+ of players, load in under 10 seconds, and have a build size below 20 MB". Load time is measured until the SDK `gameplayStart` call. They advise loading the first level first and streaming the rest. — [CrazyGames docs: basic launch metrics](https://docs.crazygames.com/resources/basic-launch-metrics/); [Getting to the first frame](https://docs.crazygames.com/resources/getting-to-the-first-frame/)
- Poki developer docs: "The amount of players who drop off during loading shouldn't be underestimated." Show a visual loading indicator so the game doesn't look frozen. — [Poki for Developers](https://developers.poki.com/guide/easy-access)
- Poki 2026 State of Web Gaming (commissioned survey: 2,000 players and 400 developers in the UK/US, May 2026). Poki reports **100M+ monthly players in 2026, up from 10M in 2020**. More than a third of web gamers play multiple times a day. 62% have bought or downloaded a game after first playing it on the web. 53% of mobile studios plan to port to browser within 12 months. — [Poki report](https://poki.com/blog/state-of-web-gaming-report-2026); [Game Developer press release](https://www.gamedeveloper.com/press-release/new-study-reveals-the-growth-engagement-discoverability-and-value-driving-web-gaming-to-outperform-gaming-giants-and-social-media); [PocketGamer.biz](https://www.pocketgamer.biz/report-53-plan-to-port-mobile-games-to-browser-in-next-12-months/). Caveat: the report is commissioned by an interested party.
- Coverage of the report is headlined "Web Gamers Quit Slow-Loading Apps". — [Sentinel Assam](https://www.sentinelassam.com/cities/guwahati-city/web-gamers-quit-slow-apps-as-browser-play-gains-on-social-media)
- Wordle: no ads, no data collection ("that is also quite deliberate"), free, and no app at launch. Wardle said "people have an appetite for things that transparently don't want anything from you." — [TechCrunch](https://techcrunch.com/?p=2256733); [GamesRadar](https://www.gamesradar.com/wordle-creator-wants-the-viral-guessing-game-to-stay-simple-and-ad-free); [TechSpot](https://www.techspot.com/news/92887-viral-online-game-wordle-stay-ad-free-no.html)
- Wordle wasn't launched as an app partly because Wardle found Android development hard. He nearly built an Android app in 2013. — [Genbeta](https://www.genbeta.com/web/wordle-no-fue-lanzado-como-app-porque-wardle-su-creador-se-le-da-fatal-programar-android-esta-otras-9-curiosidades-que-ha-desvelado-conferencia); [Android Central](https://www.androidcentral.com/apps-software/josh-wardle-tried-to-make-wordle-android-app-2013)
- Neal Agarwal: projects took off once consolidated on a single domain (neal.fun). He prefers the web to app stores, since a satirical game mocking Apple wouldn't pass App Store review. He is the only full-time person and earns his living from site ads. — [Working Theorys interview](https://www.workingtheorys.com/p/the-craft-neal-agarwal); [Wikipedia](https://en.wikipedia.org/wiki/Neal_Agarwal)

### Inferences
Friction checklist:
- First interactive frame in under 3–5s on mobile 4G, with an initial payload of a few MB.
- No signup gate. Store progress and streaks in `localStorage`, with optional account sync later.
- Rules learnable in one attempt; Wordle's colored tiles teach themselves.
- Portrait-mobile-first layout and tap targets, since shared links are mostly opened on phones.
- A single memorable URL or domain builds a brand and a return habit (neal.fun).
- Low friction compounds virality. The link-click → play gap is where shared-link traffic is lost.

### Gaps
- No controlled study (outside portal vendor data) on load time vs. retention specific to games was found.
- No data comparing signup-gated vs. ungated casual-game retention was found.

## 5. Academic and industry research frameworks (SDT, Hooked, flow, variable-ratio reinforcement, GDC talks, Wordle studies)

### Takeaway
Self-Determination Theory (Ryan, Rigby & Przybylski 2006) is the best-supported academic account of why games are enjoyable: satisfying autonomy, competence and relatedness predicts enjoyment and future play. It does *not* explain problematic play. Variable-ratio reinforcement and Hooked explain persistence but sit closest to gambling. Peer-reviewed Wordle-specific research is thin; most "Wordle psychology" is 2022 expert commentary.

### Cited Findings
- Ryan, Rigby & Przybylski (2006), "The Motivational Pull of Video Games: A Self-Determination Theory Approach", *Motivation and Emotion*: four studies found that perceived in-game **autonomy and competence** are associated with enjoyment, preference, and changes in well-being. **Autonomy, competence and relatedness independently predict enjoyment and future play.** In MMOs, relatedness supported presence and intent to keep playing. — [Springer PDF](https://link.springer.com/content/pdf/10.1007%2Fs11031-006-9051-8.pdf); [ScienceDaily 2006](https://sciencedaily.com/releases/2006/12/061226134706.htm)
- Limitation: Mills et al. found needs satisfaction explains the appeal of games but **does not meaningfully explain problematic gaming**. — [Carleton GOAL Lab PDF](https://carleton.ca/goallab/wp-content/uploads/Exploring-the-Pull-and-Push-Underlying-Problem-Video-Game-Use_-A-Self-Determination-Theory-Approach.pdf)
- Hooked model (Eyal 2014): trigger → action → variable reward → investment. Its variable-reward phase is compared to a slot machine. — [Medium / Behavior Design](https://medium.com/behavior-design/hooked-on-loot-boxes-how-design-gets-us-addicted-79c45faebc05)
- Variable-ratio schedules underpin both gambling and loot boxes. — [Australian Senate](https://aph.gov.au/Parliamentary_Business/Committees/Senate/Environment_and_Communications/Gamingmicro-transactions/Report/c03); [GambleAware report](https://www.gambleaware.org/media/jmppmnee/gaming_and_gambling_report_final.pdf)
- Near-miss neuroscience: Clark et al. 2009. — [PMC](https://pmc.ncbi.nlm.nih.gov/articles/PMC2658737)
- Flow and DDA: Chen / *flOw*. — [Engadget](https://www.engadget.com/2006-09-12-flow-in-games-an-interactive-thesis-on-dynamic-difficulty.html)
- Game feel survey (Pichlmair & Johansen). — [arXiv 2011.09201](https://arxiv.org/abs/2011.09201)
- Idle-game taxonomy (Alharthi et al.). — [NSF PAR](https://par.nsf.gov/servlets/purl/10061230)
- GDC talks: Wardle, "Wordle: Doing the Opposite of What You're Meant To" (2022) ([GDC Vault](https://www.gdcvault.com/play/1027882/css/home.css)); Jonasson & Purho, "Juice It or Lose It" (2012) ([GDC Vault](https://gdcvault.com/play/1016487/contactUs)). Wardle also revealed that the 2013 word list was much harder, including words like ZIZEL and GOLPS, and he curated it down to common words. — [Axios](https://www.axios.com/2022/03/25/wordle-wordlist-josh-wardle-gdc); [PC Gamer](https://www.pcgamer.com/wordles-original-word-list-included-zizel-and-golps)
- Wordle-specific: no peer-reviewed controlled study was found. The available pieces are commentary by Tufts (desirable difficulty), Calgary (Pexman: Scrabble research as a proxy; cognition plus social interaction), SNHU (scarcity) and Psychology Today (feedback plus sharing). — [Tufts](https://now.tufts.edu/2022/01/27/what-our-brains-do-when-we-play-wordle); [UCalgary](https://ucalgary.ca/news/wordle-craze-why-do-we-love-puzzles-and-are-they-good-our-brains-0); [SNHU](https://www.snhu.edu/about-us/newsroom/hot-topics/psychology-of-wordle); [Psychology Today](https://psychologytoday.com/nz/blog/the-asymmetric-brain/202201/the-psychology-behind-wordle)

### Inferences
- SDT gives a "healthy" design compass. **Competence:** clear feedback, fair difficulty, visible mastery. **Autonomy:** meaningful choices and no coercion. **Relatedness:** a shared puzzle, comparing results, communities. Wordle hits all three in 3 minutes.
- Hooked and variable-ratio reinforcement explain compulsion, but they also mark where the risk of manipulation lies.
- Wordle's word-list curation is a mastery-curve lesson: lower obscurity so success feels earned, not arbitrary.

### Gaps
- *A Theory of Fun* (Koster) and *Hooked* (Eyal) primary texts were not retrieved; only summaries were.
- No 2024–2026 peer-reviewed study on daily-puzzle games was found in this session.

## 6. Engaging vs. manipulative: dark patterns and ethical guidelines

### Takeaway
The standard academic reference is Zagal, Björk & Lewis (2013), "Dark Patterns in the Design of Games". It covers **temporal** (grinding, appointment play / play longer than you want), **monetary** (pay-to-skip) and **social** (social pyramid schemes) patterns, and a later study added a psychological category. The framework has been criticized for lacking an explicit ethical basis. Wardle's stated "respect your time" philosophy is the clearest practitioner counter-model.

### Cited Findings
- Zagal, Björk & Lewis (FDG 2013) define "dark game design patterns" as questionable, perhaps unethical. They intend to contribute to discussion of values in games, not to criticize creators. — [Chalmers](https://research.chalmers.se/en/publication/177148); [deceptive.design summary](https://deceptive.design/articles/dark-patterns-in-the-design-of-games)
- Categories: temporal (grinding; appointment play; making people play longer than they want), monetary (pay-to-skip), social-capital (social pyramid schemes). Later work added a psychological category. — [arXiv 2412.05039](https://arxiv.org/html/2412.05039v1); [arXiv 2401.06247](https://arxiv.org/pdf/2401.06247)
- Critique: "Against 'Dark Game Design Patterns'" (DiGRA 2020) says the original doesn't specify its ethical framework, and that it implicitly treats unflagged patterns as value-neutral. It proposes consequentialist, virtue-ethics or care-ethics lenses. — [White Rose eprints](https://eprints.whiterose.ac.uk/156460/1/DiGRA_2020_paper_189.pdf)
- Loot boxes: there is a link between problem-gambling severity and loot-box spending. Empirical research is still sparse ("dearth"; "almost no academic literature" on motivations). — [PMC7882574](https://pmc.ncbi.nlm.nih.gov/articles/PMC7882574); [Kao, MIT](https://people.csail.mit.edu/dkao/pdf/kao2019tog.pdf); [GambleAware](https://www.gambleaware.org/media/jmppmnee/gaming_and_gambling_report_final.pdf)
- The FTC economics paper frames loot-box harm as a disputed question. Industry argues loot-box spending reflects enjoyment. — [FTC](https://www.ftc.gov/system/files/ftc_gov/pdf/simonovamano.pdf)
- SDT needs satisfaction explains healthy appeal, while problematic play is driven by other ("push") factors. — [Carleton GOAL Lab](https://carleton.ca/goallab/wp-content/uploads/Exploring-the-Pull-and-Push-Underlying-Problem-Video-Game-Use_-A-Self-Determination-Theory-Approach.pdf)
- Wardle's practitioner ethic: no ads, no data harvesting, no push notifications, three minutes a day, "doesn't want anything from you". — [TechCrunch](https://techcrunch.com/?p=2256733); [GamesRadar](https://www.gamesradar.com/wordle-creator-wants-the-viral-guessing-game-to-stay-simple-and-ad-free)
- Streak criticism: user-experience writers argue Duolingo-style streaks can create anxiety, and propose flexible or healthier reframings. People also report giving up long streaks. — [UX Collective](https://uxdesign.cc/3-reframing-streaks-on-duolingo-5-ideas-for-a-more-healthy-and-flexible-approach-to-language-8fd89545771e); [Android Authority](https://www.androidauthority.com/reasons-give-up-duolingo-streak-3543009)
- Near-miss effects are a known gambling mechanic, and the evidence is mixed. — [Clark 2009](https://pmc.ncbi.nlm.nih.gov/articles/PMC2658737); [PMC7214505](https://pmc.ncbi.nlm.nih.gov/articles/PMC7214505)

### Inferences
A practical line for a solo developer: ask whether the mechanic serves the player's goals (fun, mastery, connection) or extracts time and money against their reflective preferences.
- **Engaging (generally fine):** a daily cap; streaks *with* forgiveness; honest near-misses from skill; juice; personal bests; spoiler-free sharing; opt-in reminders.
- **Gray zone:** streak-loss guilt messaging; notification nagging; "appointment" timers that punish absence; idle games that need constant check-ins.
- **Dark:** fake or rigged near-misses; paid randomized rewards (loot boxes) aimed at minors; pay-to-skip artificial waits; social pyramid schemes (invite N friends to progress); confirmshaming; hidden odds; forced accounts for data harvesting.
- Wordle and Duolingo show both ends. Both use streaks. Wordle caps time and asks for nothing, while Duolingo adds monetized streak repair and pressure messaging.

### Gaps
- No formal industry code of conduct specific to casual browser game design was found. Relevant regulatory threads (e.g., UK/EU loot-box guidance, the EU Digital Fairness Act discussions, FTC dark-pattern enforcement) were not retrieved in this session.
- No 2024–2026 academic paper specifically on streak ethics was found.
