# Building, Launching and Monetizing a Solo Browser Game (2026)

Research note: WebFetch could not reach poki.com, sdk.poki.com, dev.to or developers.reddit.com from this session, so several findings rely on search-result summaries of those pages rather than full reads. Those are flagged where it matters. Some search results pointed to unofficial mirror domains (e.g., a trycloudflare.com copy of Reddit's Devvit docs); figures that appeared only there are excluded or flagged.

## Q1. Which tech stacks fit small browser games in 2026?

### Takeaway
Phaser is the default pick for a beginner making a complete 2D browser game (most tutorials, built-in physics, Phaser 4 released April 2026). Kaplay (the community fork of Kaboom) is good for jams and quick prototypes. PixiJS is a renderer, not a game framework. A daily word or logic puzzle needs no engine at all: plain HTML/CSS/JS plus a small backend is enough. AI coding assistants can produce a shippable browser game quickly, but the well-known "vibe coded" success leaned on a huge existing audience.

### Cited Findings
- Phaser 4.0 ("Caladan") shipped April 11, 2026; Phaser includes three physics systems (Arcade, Impact, Matter.js) and is widely described as beginner-friendly — [pistack.xyz comparison](https://www.pistack.xyz/posts/2026-08-18-phaser-vs-pixijs-vs-kaboom-javascript-game-engine-comparison/); [Cinevva engine guide](https://app.cinevva.com/guides/web-game-engines-comparison.html)
- Phaser's own April 2026 comparison (Phaser vs Kaplay vs Excalibur) claims Phaser handles Safari better and works better with AI coding assistants. This is vendor-written, so weigh accordingly — [Phaser news](https://phaser.io/news/2026/04/phaser-vs-kaplay-vs-excalibur-2d-web-game-framework)
- Replit no longer maintains Kaboom; its README points to the community fork KAPLAY. Verdict from one comparison: Kaplay is "a great choice for prototypes, jams, and teaching" but a poor choice for a long-lived production game without a migration plan — [pistack.xyz](https://www.pistack.xyz/posts/2026-08-18-phaser-vs-pixijs-vs-kaboom-javascript-game-engine-comparison/)
- PixiJS "isn't a game framework; it's a library for 2D rendering"; guidance: if the product is a game, start with Phaser, and use PixiJS when rendering is the product — [OpenReplay engines compared](https://blog.openreplay.com/javascript-game-engines-compared/); [Cinevva](https://app.cinevva.com/guides/web-game-engines-comparison.html)
- Wordle clones are commonly built with zero dependencies in vanilla JavaScript — [HackerNoon: zero-dependency Wordle clone](https://hackernoon.com/how-i-built-a-zero-dependency-wordle-clone-with-vanilla-javascript)
- AI-built example: Pieter Levels' fly.pieter.com, a browser 3D multiplayer flight sim built with AI help (his blog describes Python websockets for multiplayer), launched Feb 2025 and claimed $1M ARR in 17 days ($87K MRR, a run-rate, not cash collected) — [levels.io](https://levels.io/full-multiplayer-python-websockets-game-ai); [DEV write-up](https://dev.to/promptway/he-built-a-flight-simulator-in-three-hours-and-hit-1m-a-year-in-17-days-then-it-went-to-zero-1b1l)
- By May 2025 it had dropped to about $12K MRR — [Indie Hackers roundup](https://www.indiehackers.com/post/2NUIOp80SUWuPmmfKoS9). A DEV piece claims it later reads "$0/m" in his bio (secondary, unverified) — [DEV](https://dev.to/promptway/he-built-a-flight-simulator-in-three-hours-and-hit-1m-a-year-in-17-days-then-it-went-to-zero-1b1l). Commentators attribute much of the success to his 600K+ X followers — [404 Media](https://404media.co/this-game-created-by-ai-vibe-coding-makes-50-000-a-month-yours-probably-wont)
- Reddit and Phaser ran a $40,000 "Games with a Hook" hackathon in June–July 2026 for games on Reddit's Devvit platform; 3,071 registrants and 700+ games submitted. Phaser is a supported engine there — [Phaser news](https://phaser.io/news/2026/06/reddit-and-phaser-launch-a-40-000-game-dev-hackathon); [winners post](https://phaser.io/news/2026/08/games-with-a-hook-hackathon-phaser-winners)

### Inferences
- Daily puzzles (word, logic, trivia, grid) fit plain HTML/CSS/JS or a light UI framework, since the game is mostly DOM state, and the main engineering work is the backend for daily answers and streaks. Action, arcade and .io games fit Phaser (2D) or Three.js (3D), with a websocket or Durable Objects backend for multiplayer.
- For a beginner using an AI assistant, Phaser has a big advantage: it has the most code in public, so assistants generate working Phaser code more reliably. The Phaser team says the same, but that claim is self-interested.
- The fly.pieter.com arc (spike, then decay) shows that AI makes building cheap. Distribution and retention are still the hard part.

### Gaps
- I found no solid 2026 source comparing Godot 4 web export (bundle size, load times, Safari/iOS issues, portal acceptance) with JS frameworks. Treat Godot web as "works, but larger downloads and more friction" only as an unverified generalization.
- I didn't research Three.js-specific beginner guidance separately.

## Q2. Where can games be hosted cheaply, and what backend is needed?

### Takeaway
Static hosting for the game client is effectively free (GitHub Pages, Cloudflare Pages, Netlify, Vercel). Daily puzzles and leaderboards need a small backend: Supabase's free tier works but pauses after about a week of inactivity, and Cloudflare Workers plus Durable Objects now has a free tier that Cloudflare itself pitches for multiplayer games. The caps are tight: 100K requests/day and 10 ms CPU per request.

### Cited Findings
- Supabase Free plan projects are paused after a period of low database activity (third parties describe it as about 7 days); owners get a warning email about a week before. Pro plan removes pausing — [Supabase docs: project pausing](https://supabase.com/docs/guides/platform/free-project-pausing); [Supabase KB](https://supabase.com/kb/faqs/platform/free-project-pausing)
- Supabase free limits per third-party 2026 summaries: 500 MB database, 1 GB file storage, 5 GB bandwidth, 50,000 MAU, 2 free projects. Confirm on supabase.com/pricing — [automationatlas.io](https://automationatlas.io/answers/supabase-free-tier-limits-2026/); [Activepieces](https://www.activepieces.com/blog/supabase-pricing-free-tier-limits-pro-costs-egress)
- Cloudflare Durable Objects became available on the Workers Free plan in April 2025, with multiplayer games named as a use case. Free accounts must use SQLite-backed Durable Objects — [Cloudflare changelog](https://developers.cloudflare.com/changelog/2025-04-07-durable-objects-free-tier); [DO pricing](https://developers.cloudflare.com/durable-objects/platform/pricing)
- Workers Free: 100,000 requests/day, 10 ms CPU per request; limits reset at 00:00 UTC, and requests over the limit fail. Free plan DO storage is capped at 5 GB total — [Workers pricing](https://developers.cloudflare.com/workers/platform/pricing/); [Durable Objects limits](https://developers.cloudflare.com/durable-objects/platform/limits)
- CrazyGames offers a built-in leaderboards SDK with server-side validation — [CrazyGames docs: leaderboards](https://docs.crazygames.com/sdk/leaderboards-client/)

### Inferences
- A good free stack for a daily puzzle: client on Cloudflare Pages or GitHub Pages, and a Cloudflare Worker that serves "today's puzzle ID" and checks guesses, with puzzle data in D1/KV or Supabase. A Worker never sleeps the way a free Supabase project does.
- For a solo student, the daily 100K-request cap is roughly the point where a game is successful enough that $5/month for Workers Paid is easily justified.
- If a game launches through Poki or CrazyGames, the portal hosts it, so self-hosting matters mainly for a standalone domain.

### Gaps
- I didn't verify current Cloudflare Pages, Vercel, Netlify or GitHub Pages bandwidth/build caps from primary docs. Vercel's Hobby plan prohibits commercial use per its terms, which matters if the site runs ads, but I did not re-verify this in 2026.
- Firebase free-tier (Spark) limits not researched.

## Q3. Monetization options and what they pay

### Takeaway
For a solo dev, the realistic money paths are: (1) a web portal revenue share (Poki, CrazyGames), (2) display ads on your own domain for a daily game that retains users, and (3) platform programs like Reddit Developer Funds. Most indie web games earn little. Success stories run from a few thousand dollars a month (Actorle at about $4K/month) up to full-time studio income on Poki, with one-off acquisitions (Wordle to NYT, low seven figures) being rare outliers.

### Cited Findings
**Web portals**
- Poki: developer gets 100% of earnings when the developer brings the player (search, direct) and 50% when Poki brings the player via its promotion; Poki uses revenue share, not upfront fees (search summary of Poki's deals/SDK pages; could not fetch directly) — [Poki SDK deals](https://sdk.poki.com/deals); [Poki SDK](https://sdk.poki.com/). A comparison site says portals negotiate per game and percentages aren't universal — [Playgama comparison](https://playgama.com/blog/business-faqs/poki-vs-crazygames-vs-gamedistribution-revenue-share/)
- Poki success stories: Blumgi reached 100M players in 2 years as a solo indie — [Poki blog, Sep 2023](https://poki.com/blog/blumgi-my-journey-on-the-web-how-i-reached-100m-players-in-2-years-as-an-indie-game-developer), follow-up May 2026 — [Poki blog](https://poki.com/blog/developer-spotlight-blumgi-games-part-2); Emolingo Games built a business on HTML5 web games via Poki — [Poki blog, Jul 2025](https://poki.com/blog/how-emolingo-games-built-business-html5-web-games-poki); an indie earning close to six figures from two games — [Exputer](https://exputer.com/?p=445036). A claim that top Poki games earn up to €1M/yr (citing Dealroom) is unverified — [Cinevva](https://app.cinevva.com/guides/web-game-monetization)
- Poki has passed 1 billion monthly plays — [Tech Funding News](https://techfundingnews.com/browser-gaming-website-poki-won-big-at-the-dutch-game-awards-celebrating-hitting-1-billion-monthly-plays/)
- CrazyGames: main model is ad revenue share; no official split in its main docs. A 2026 GameMaker jam's terms listed 60% of ad revenue and 70% of in-game purchases to devs (jam-specific, not necessarily general). Payouts are monthly via Tipalti with a €100 minimum (secondary source) — [CrazyGames docs](https://docs.crazygames.com); [Cinevva CrazyGames guide](https://app.cinevva.com/guides/publish-game-crazygames); [CrazyGames ad monetization guide](https://docs.crazygames.com/resources/ad-monetization-guide/)

**Own-site ads / daily games**
- Actorle (daily actor-guessing game, built as a 3-day side project) still made about $4,000/month two years after launch with minimal upkeep (self-reported) — [hey.gg](https://hey.gg/blog/actorle); [Indie Hackers](https://www.indiehackers.com/post/how-did-i-create-a-game-with-4-000-monthly-revenue-in-3-days-49b598a252)
- Flagdoku (daily flag puzzle) had erratic ad revenue before switching ad providers to Playwire — [Playwire case study PDF](https://www.playwire.com/hubfs/%5BCase%20Study%5D%20Flagdoku%20-%20Google%20Docs.pdf)
- A web game post-mortem reports hitting 130K MAU with zero marketing and surviving an AdSense ban (title-level only; page could not be fetched). It is a warning that a single ad-network account is a risk — [DEV post-mortem](https://dev.to/yitao/post-mortem-how-my-web-game-hit-130k-mau-with-0-marketing-and-survived-an-adsense-ban-883)
- Solitaire site grown to $10K MRR; commenters say most income was ads and players don't pay for solitaire — [Indie Hackers](https://www.indiehackers.com/post/how-i-grew-a-simple-solitaire-game-to-10k-mrr-28e352c308)
- fly.pieter.com mixed in-game sponsor ads (~$5,000/month per placement) with a $29.99 premium plane purchase — [404 Media](https://404media.co/this-game-created-by-ai-vibe-coding-makes-50-000-a-month-yours-probably-wont); [Indie Hackers](https://www.indiehackers.com/post/2NUIOp80SUWuPmmfKoS9)

**Patreon / Ko-fi**
- Patreon takes 8–12% plus processing; average creator earnings are cited as $315–$1,575/month (aggregator source, not game-specific) — [FinanceBuzz](https://financebuzz.com/how-to-make-money-with-patreon)

**Selling to publishers**
- NYT bought Wordle in January 2022 for "low seven figures" — [NPR](https://www.npr.org/2022/01/31/1077089945/nyt-wordle); [PC Gamer](https://pcgamer.com/wordle-sells-to-the-new-york-times-for-a-seven-figure-sum). No 2025–2026 NYT acquisition of an indie puzzle game turned up in search.

**Platform programs**
- Reddit Developer Funds (Devvit): engagement-milestone payouts. A March 2025 r/Devvit thread listed tiers like 500 daily qualified engagers for $500, 1,000 for $1,000, up to 10,000 for $5,000; apps that already got a payout may be ineligible — [r/Devvit thread (mirror)](https://libreddit.winscloud.net/r/Devvit/comments/1jlhi8b/the_continuation_of_reddit_developer_funds). Reddit's own docs page could not be fetched; check developers.reddit.com for 2026 tiers. Hackathon prizes (e.g., $40K pool in 2026) are another route — [Phaser news](https://phaser.io/news/2026/06/reddit-and-phaser-launch-a-40-000-game-dev-hackathon)
- Discord Activities: opened to all developers; Activities devs can use Premium Apps (durable/consumable SKUs). Monetization launched for US, UK, and EU devs on desktop — [Discord blog](https://discord.com/blog/build-where-the-world-plays); [PocketGamer.biz](https://www.pocketgamer.biz/discord-activities-opens-up-to-all-developers-to-make-games-on-the-platform). A Discord newsroom snippet mentions a 15% fee on the first $1M (context unconfirmed) — [Discord newsroom](https://discord.com/newsroom)
- YouTube Playables: revenue sharing is still a pilot with "a select number" of creators; no open self-serve revenue share — [Google Developers: Playables monetization](https://developers.google.com/youtube/gaming/playables/reference/monetization). Third-party publishers (e.g., Playgama) distribute to Playables under their own splits — [Playgama](https://playgama.com/blog/business-faqs/how-do-i-publish-a-game-on/)

### Inferences
- For this user, the most realistic first dollars come from either a Reddit Devvit daily game (Developer Funds milestones plus hackathons, built-in distribution) or a Poki/CrazyGames submission of a polished Phaser arcade game. Own-domain AdSense needs sustained daily traffic before it pays meaningfully.
- Daily puzzles monetize through habit (ads on every return visit), while .io/action games depend on portal traffic.
- Diversify ad networks; one AdSense ban can zero out revenue.

### Gaps
- No verified 2026 eCPM figures for web game display ads or rewarded ads.
- I didn't find whether LinkedIn's games (Queens, Pinpoint, etc.) came from outside acquisitions; there is no evidence that LinkedIn buys indie games.
- No direct earnings reports for Ko-fi, premium tiers, or sponsorships beyond fly.pieter.com.

## Q4. Launch and distribution tactics

### Takeaway
Browser-playable builds get far more plays than downloads, and r/WebGames can kick off a puzzle game's growth (Rogule). Generic multi-subreddit posting often flops. Show HN, TikTok and Product Hunt evidence is thin in the sources found.

### Cited Findings
- Rogule (daily roguelike) was posted to r/WebGames a month after creation, was picked up and "snowballed" to about 2,000 daily players — [Indie Hackers](https://www.indiehackers.com/post/2000-people-per-day-are-playing-rogule-cf104c6362)
- A browser MOBA posted to 5 subreddits got 3 upvotes total; one post was removed for breaking r/Games' Indie Sunday rules. Suggestions included scheduled "play with the dev" sessions — [Indie Hackers](https://www.indiehackers.com/post/i-posted-my-browser-moba-shooter-to-5-subreddits-and-got-3-upvotes-then-i-gave-it-a-map-editor-8038535a59)
- On itch.io, browser-playable games draw roughly 3x more players than downloadable ones; another dev reports about 10x — [How To Market A Game: itch.io benchmark](https://howtomarketagame.com/2025/05/12/benchmark-itch-io-traffic/)
- Game jams with real prize pools: Reddit x Phaser 2026 hackathon ($40K, 700+ entries) — [Phaser](https://phaser.io/news/2026/08/games-with-a-hook-hackathon-phaser-winners); CrazyGames-linked GameMaker web jam (2026) — [Cinevva](https://app.cinevva.com/guides/publish-game-crazygames)
- A Product Hunt browser-games platform reported a milestone of 121K active users — [Product Hunt](https://www.producthunt.com/p/the-first-ai-driven-free-gaming-platform/milestone-121k-active-users-4-6m-events-on-our-ad-free-browser-games-platform)
- Wordle-style emoji share grids drove virality (the NYT acquisition coverage notes its spread) — [TIME](https://time.com/6143832/new-york-times-buys-wordle)

### Inferences
- Recommended sequence: put a free build on itch.io or a jam, post to the niche subreddit that matches the game (r/WebGames, r/incremental_games, r/wordle-type subs) following each sub's self-promo rules, then do Show HN once the game is polished. A shareable result grid is built-in marketing for a daily puzzle.

### Gaps
- No sourced 2026 data on Show HN, TikTok or short-video launch results for browser games. Poki's "State of Web Gaming Report 2026" (June 2026) exists but couldn't be fetched — [Poki blog](https://poki.com/blog/state-of-web-gaming-report-2026).

## Q5. Cheating and security for daily puzzles and leaderboards

### Takeaway
Wordle shipped its whole answer list in client JS, which let anyone read future answers. The fix is to keep answers server-side and return only per-guess feedback. For leaderboards, never trust a client-submitted score. Submit inputs or replays with a server-issued RNG seed and re-simulate server-side, then add rate limits and sanity checks. Obfuscation only slows casual cheaters. This is a good portfolio angle for a cybersecurity student.

### Cited Findings
- Wordle's 2,315 answers were stored in plaintext, in daily order, in its client-side JS, with no server check of answers — [PCWorld](https://www.pcworld.com/article/606109/how-to-cheat-at-wordle.html); [The Conversation](https://theconversation.Com/wordle-has-been-hacked-but-thats-not-going-to-ruin-the-fun-175675); [Medium: re-hacking Wordle](https://medium.com/@capJavert/re-hacking-wordle-114ba75d1344)
- Server-backed clone pattern: keep game state and answer on the server and return only per-letter evaluation; scoring needs two passes to handle duplicate letters — [jakerella/guessle](https://github.com/jakerella/guessle); [Coteh/wordle-clone](https://www.github.com/Coteh/wordle-clone)
- In the browser, game logic, score and the submission request are all visible and editable in devtools — [gamedev.net thread](https://gamedev.net/forums/topic/710630-preventing-users-spoofing-messages-to-backend-from-javascript/5441680); [Playgama: client-side leaderboard cheating](https://playgama.com/blog/business-faqs/how-to-prevent-cheating-on-client-side-leaderboards-in-html5/)
- Open Hexagon sends replay files (timestamps plus inputs) to the server, which verifies them before ranking. Its developer admits slow-down cheat tools can still inflate scores — [GIGAZINE](https://gigazine.net/gsc_news/en/20211110-open-hexagon-against-cheet)
- Server-authoritative pattern for a prize game: server-issued RNG seed, server re-simulates the run, replayed requests rejected as duplicates. The developer found exact replay matching hard because of UI/state bugs — [DEV: Don't trust the score](https://dev.to/gowtham_r_2002/dont-trust-the-score-building-server-authoritative-validation-for-a-prize-based-mobile-game-246i)
- Extra layers: HMAC-signed submissions, checks that event counts match scores, monotonic timestamps, rate limits; obfuscation only deters casual tampering — [Playgama](https://playgama.com/blog/business-faqs/how-to-prevent-cheating-on-client-side-leaderboards-in-html5/); [Unipop devlog: Re: Hacking the Leaderboards](https://javacakegames.itch.io/unipop/devlog/306546/re-hacking-the-leaderboards)
- CrazyGames' leaderboard always returns success to the client and validates scores on its backend, so cheaters can't probe which submissions are rejected — [CrazyGames docs](https://docs.crazygames.com/sdk/leaderboards-client/)

### Inferences
- A daily puzzle with a server-only answer, a Worker endpoint that grades guesses, and rate limiting per IP/session is easy for a beginner to build and gives a concrete security story to write up for a portfolio, such as a blog post on threat-modeling a Wordle clone.
- Speedrun/time leaderboards for puzzles can be partly checked by requiring the server to timestamp puzzle-start and puzzle-solve events, rejecting impossible times.
- For hobby games, "good enough" anti-cheat means silent rejection plus anomaly review. Perfect prevention isn't achievable client-side.

### Gaps
- No quantified data on how common leaderboard cheating is in indie web games.
