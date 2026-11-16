# App idea: plan + tools log
**Read this first in any chat about the app. Update it at the end of every session.**
Started 2026-11-15. Status: **idea stage. No app idea chosen yet, nothing built.**

---

## 1. The goal
- Build a phone app, publish it on the **App Store** (and Google Play), make money with **subscriptions**, promote it on **TikTok and Instagram**.
- Covers everything: making it → design → login → payments/subscriptions → security → store listing → promotion.
- Fits the bigger plan: $3K/month by end of 2027 (see `../2027-PLAN.md`). The app comes after the AI-tips account is running.

## 2. Decisions already made
| Topic | Decision | Why |
|---|---|---|
| How to build | **Expo (React Native)**: one codebase for iPhone + Android | The laptop is Windows. Expo's **EAS** builds the iPhone version in the cloud, so no Mac is needed |
| Login + database | **Supabase** (plugin already installed) | Login (email, Apple, Google) + database + storage in one |
| Payments / subscriptions | **RevenueCat** | The standard for app subscriptions; handles Apple + Google billing and paywalls |
| Website / landing page | Vercel (plugin installed), same black-and-white style as the EIGHTYSIX site | Site at `../ai-account/site/` |
| Security | security-and-hardening + security-review skills before every release | Protects user data and keys |
| Skills policy | Install skills **only when needed**; read every skill's files before installing | More skills = more confusion + more risk |

## 3. Costs to expect
| What | Cost | When |
|---|---|---|
| Apple Developer Program | **$99 / year** | Before the first App Store upload |
| Google Play developer account | **$25 once** | Before the first Play Store upload |
| Expo EAS builds | Free tier has monthly build limits; paid if we need more | During building |
| Supabase | Free tier to start | From day 1 |
| RevenueCat | Free until the app earns a set amount per month (check their current terms) | When we add subscriptions |
| Apple/Google cut on subscriptions | About 15–30% of each payment | After launch |
(Verify the prices on each site before paying; they can change.)

## 4. The roadmap (steps, in order)
1. **Pick the idea.** Problem, who it's for, why they'd pay. Optional: run it through Roast Room (`C:\Users\Laptop\roast-room`, `/roast-room ...`).
2. **Study competitors.** Find 3–5 apps doing something similar: what they charge, their reviews, their weak spots (skills: `aso`, REA once installed).
3. **Clickable demo first.** A fake but clickable version to test the idea and use in reels (fil.design skill once installed).
4. **Design.** Screens, colours, fonts (`expo-design-system`, `expo-native-ui`, design sites below).
5. **Build.** Expo project, screens, navigation (`expo-overview` first, then `expo-project-structure`, `expo-router`, `expo-ui`, `react-native-best-practices`).
6. **Login + data.** Supabase.
7. **Subscriptions.** RevenueCat: products, paywall, premium lock, test purchases with no real money.
8. **Security check.** `security-and-hardening`, `security-review`.
9. **Store listing.** Name, icon, screenshots, keywords (`aso`, `copywriting`).
10. **Publish.** EAS build + submit to TestFlight → App Store, and to Google Play (`eas-app-stores`, `eas-workflows`).
11. **Launch + promote.** Launch plan, TikTok/IG reels, comment-keyword DMs (`launch`, Instagram + TikTok skills, video skills).
12. **Improve.** First-session experience and pricing (`onboarding`, `pricing`, `marketing-psychology`).

## 5. Skills we have (installed)
### Building the app (Expo, official)
- `expo-overview`: load first, it routes to the right Expo skill
- `expo-project-structure`: folders for a new app
- `expo-router`: screens, tabs, navigation
- `expo-native-ui`: looks like a real iPhone app
- `expo-ui`: native buttons, sliders, sheets, menus
- `expo-design-system`: one consistent theme
- `eas-app-stores`: build + submit to App Store / Google Play
- `eas-workflows`: automate builds and releases
- `react-native-best-practices` (Vercel): speed and performance

### Payments + subscriptions (RevenueCat, official)
- `revenuecat`: general help
- `create-revenuecat-project`: products, plans, entitlements
- `integrate-revenuecat`: connect it to the app
- `revenuecat-paywall`: the "go premium" screen
- `revenuecat-entitlements-gate`: lock premium features
- `revenuecat-testing-setup`: test purchases without real money

### Login, database, web, payments outside the app (plugins already installed)
- **Supabase** plugin: login, database, storage
- **Stripe** plugin: payments on a website (not inside the iPhone app; Apple requires its own billing there)
- **Vercel** plugin: website / landing page hosting
- Note: Supabase, Stripe and Vercel each need to be connected once (sign-in) before first use.

### Security
- `security-and-hardening`, `security-review`

### Design
- `frontend-design`, `website-builder-setup`, `design-and-templates`
- Saved design websites (use only when you say so): 21st.dev, reactbits.dev, magicui.design, uiverse.io, mobbin.com (inspiration), styles.refero.design (ready style guides for AI). Not checked yet: designeer.xyz, inspora.design.

### Marketing (installed 2026-11-15)
- `aso`: App Store search ranking
- `launch`: launch plan
- `pricing`: what to charge
- `onboarding`: first screens that keep users
- `copywriting`: headlines and text that sell
- `marketing-psychology`: why people buy

### Promotion on TikTok + Instagram (already had)
- Instagram skills: `ig-reel`, `ig-caption`, `ig-viral`, `ig-audit`, `ig-plan`, `ig-story`, `ig-profile`, `ig-dm`...
- Social-media skills (70+): `tiktok-script`, `tiktok-growth`, `tiktok-video-publishing`, `instagram-growth`, `short-form-video-script`, `hook-writer`, `lead-magnets-and-funnels`...
- Reading reels and accounts: Agent Reach, yt-dlp, vidIQ connector
- Comment-to-DM: ManyChat (same setup as `../emilia-series/freebie/MANYCHAT_SETUP.md`)

### Making promo videos (already had)
- **Hypit**: copy a viral reel's structure, free code-only mode (test: `../ai-account/tests/hypit-clone/`)
- **cinematic-film**: documentary "evidence wall" style (test: `../ai-account/tests/medusa/`)
- **HyperFrames**, Remotion, Lemo Opuscar, `saas-master` (product promo videos), plus stick-figure, anime, paper-cutout, pixel-art and others

### Deciding
- **Roast Room**: council of business advisors for big decisions (`C:\Users\Laptop\roast-room`)

## 6. Skills to install LATER (when we start the app)
From @mengto's Threads post (2026-11-15):
- ✅ **Emil Kowalski's skills** (emilkowal.ski/skill): premium animations and interactions
- ✅ **REA, Reverse Engineer Anything**: how any app or site works (competitor study)
- ✅ **fil.design skill**: clickable live demo of the app in HTML
- 🟡 **hairline** (hairline.lucasmarkes.com): line drawings for the website
- 🟡 **Meng To's skills** (github.com/mengt…): need the full link
- ❌ github.com/achim… (Blender + AI images): skip, already covered

## 6b. Free guides to follow (Nelson Builds, nels-ysng-guides.vercel.app)
Free PDFs, no signup. Read each one when we reach that step, not before. (The paid "Idea to App Store" guide is £19.99; not needed yet.)
| Roadmap step | Guide | Key takeaways |
|---|---|---|
| 3. Demo | Idea to MVP in 1 Day | Cut to ONE core flow. No login, settings or payments on day 1. Show 2–3 people and ask: "Where did you hesitate?" |
| 4. Design | Designing UI with AI | Pick colours + font + spacing (8px) BEFORE prompting. Feed 2–3 real app screens (Mobbin) as reference. Ban the AI look: no purple gradients, no emoji icons, no centred-everything. Contrast 4.5:1, tap targets 44pt |
| 5. Build | AI Coding Stack | Same stack as ours: Expo + EAS + Claude Code. Set `"autoIncrement": true` in eas.json |
| 7. Subscriptions | Subscriptions with RevenueCat | Product IDs must match in 4 places. Use `_v1` in IDs. Configure RevenueCat at app launch, not on the paywall. Check the entitlement, never the product. A cancelled purchase is not an error. A Restore Purchases button is required |
| 9–10. Store + publish | Launching on the App Store | Privacy Policy + Terms + Support as live web pages (our Vercel site can host them). In-app account deletion is required. Sign in with Apple is required if we offer Google login. Screenshots 1320×2868, no transparency. Give reviewers a demo login |

**Where the guides don't fit us:**
- **Database:** the guides say use Firestore and avoid Supabase (cost). We keep **Supabase**: its free tier, login and plugin are already set up. Revisit only if the bill grows.
- **No Mac:** his StoreKit testing and `npx expo run:ios --device` need Xcode on a Mac. On Windows we use **EAS development builds** on the iPhone and the `revenuecat-testing-setup` skill instead.

## 6c. Reel: nels_ysng "I sold my vibe-coded app I built in 2 months" (same author as 6b)
His 4 steps (read from the on-screen text; the audio wasn't transcribed):
1. **Validate the idea.** 3 ways to find one: solve your own problem, mine Reddit and social media, **copy what already pays**. Check what an existing app earns with **Appmagic** or **Sensor Tower** (estimated revenue + downloads). His idea came from a Starter Story video ("This app made over $1M").
2. **Write a PRD** (`prd.md`): what you're building, who it's for, the problem it solves, core features, how it all works. Prompt: "turn my app idea into a prd".
3. **Build the MVP.** React Native + Expo (iOS + Android). Give the coding agent a UI reference: Mobbin, or screenshots of real apps (Pinterest / App Store). Turn off everything except **the core feature** (no social feed, AI chat, leaderboards or widgets).
4. **Backend + analytics.** Login + database, RevenueCat for subscriptions, **PostHog** for analytics (daily active users).

**What this changes in our roadmap:**
- Step 1 (pick the idea): use his 3 ways, and check the money with Appmagic / Sensor Tower.
- New step between 2 and 3: **write `prd.md`** before any demo or code.
- Step 6: add **PostHog** analytics next to Supabase (it has a free tier; check its current limits).

**Promotion lesson:** the reel itself is the model for our TikTok/IG content. The hook is a result ("I sold my app"), followed by numbered steps with big on-screen text, filmed at the desk, ending with "Comment 'App' for my guides" (a keyword-to-DM funnel, same as our ManyChat setup).

## 6d. Example account: @frist.com.de (from a screenshot, 2026-11-15)
- **What it is:** a tool that tracks finance and tech internship deadlines in Germany, Austria and Switzerland, updated daily. Its features include deadline reminders, a CV check and application tips. It's small: 8 posts and 113 followers, so it isn't proof the method works yet.
- **Their method:**
  1. **Character reels about the pain.** 3D cartoon students in relatable moments: "only a 5-minute break" while a deadline counts down, "applications: 78", "How am I supposed to know when the application opens?"
  2. **The product hides inside the joke.** The laptop in the reel shows frist's own screen (internship, deadline "today 23:59", countdown). It's an ad that doesn't feel like one.
  3. **Useful news people share.** "Deutsche Bank Spring Week. Open for 5 days. Most people don't know." This creates fear of missing out and makes people save and send the post.
  4. **One look everywhere:** green, a serif font, the "frist." logo, 2 pinned posts, and a "Stellen" (jobs) highlight.
- **For us:**
  - Promotion: show the user's pain with a character, put our app on the screen inside the joke, and add "useful news" posts.
  - App idea pattern: **"we track X for a niche, daily, and remind you"**. That's a simple app people pay for to avoid missing something.

## 6e. Example account: @hakeem_dimoz (from screenshots, 2026-11-16)
- Melbourne, 23. Bio: "building apps until $30k/mo, currently: $30k!!" 12.6K followers, 320 posts.
- **Method: a daily "DAY N" reel** (Day 1 → Day 320), filmed raw on his phone, talking to the camera. He shares wins and failures honestly ("but it went horribly", "or suspended", "REALISTIC day in my life as a 22y/o $30k/mo app founder").
- His **pinned emotional Day 1** reel has 44.1K views. Normal days get 3–9K views, so the series builds trust over time, not through one viral video.
- **Proof:** a public page on verified.revenuecat.com showing MRR $13,978, $31,523 revenue in the last 28 days, and 2,833 active subscriptions. Revenue is about 2× MRR, which suggests many users pay **yearly** upfront.
- **For us:** the "Day N" format costs nothing and fits building the app from zero. RevenueCat can show our revenue publicly later as proof.

## Decision: promote before launch (2026-11-16)
- Start a **"Day 1" build-in-public series** before the app exists.
- Collect a **waitlist** (Vercel page + ManyChat keyword). If people don't join, the idea is weak, so change it before building.
- Keep the build short (an MVP in weeks, not months). Waitlists go cold if launch is far away.

## 7. Skipped on purpose
- Instagram/TikTok **scraper** skills: need paid scraping accounts and break Instagram's rules. We already read reels with yt-dlp + Agent Reach.
- The many **"app-store-screenshots"** copies under random publisher names: duplicates of unknown quality.
- **reddit-automation**: auto-posting gets accounts banned.

## 8. Open questions (for the user)
1. What's the app idea? (Problem + who pays.)
2. iPhone only first, or iPhone + Android together?
3. Price idea: monthly subscription, yearly, or one-time unlock?
4. Will the app be promoted from @eightysix.makes, or a new account just for the app?

## Session history
- **2026-11-15:** user decided to build an app someday. Researched skills.sh; installed 21 skills (Expo ×9, RevenueCat ×6, marketing ×6); saved design sites; reviewed @mengto's skill list (install 3, 5, 6 later). This file created.
- **2026-11-15 (later):** plan saved to the `oneeye10/86` repo (push blocked until the Claude GitHub App has access). This chat's purpose: build the app and promote it on TikTok/IG to get users.
