# Newsreel app — purpose (research-derived, Aug 6 2026)

Derived from two sourced research passes through the mandated lens — Substack's app designers,
Nikita Bier, and creators who made hard daily jobs beloved (Wordle, Duolingo, Oura) — then used
as the gate to audit `app-v3.html`. Sources inline.

## The purpose

**Give a young person who quit the news the daily five-minute ritual that leaves them feeling
caught up, capable, and calm — a finite, finishable Stack told by verified humans they choose to
follow, not a feed that maximizes time-on-app.**

## Key research findings (cited)

**Substack lens.** Chris Best frames media as "Future A (The Drug)" — engagement, outrage — vs
"Future B (The Culture)" — trust, depth, direct payment (The Generalist, "Substack Playbook").
Hamish McKenzie: rival platforms are "designed to keep you trapped in an endless scroll…"
(hamish.substack.com, "Why we built a social network"). Design decisions: chronological inbox
metaphor, follows-people-not-topics, Notes ranked for subscriptions not reactions. Documented
failure modes for news: reader overwhelm ("20 subscriptions × 40+ weekly emails"), writer
marketing grind, **no daily ritual, no finish line, no shared front page**.

**Bier / hard-jobs lens.** Bier: apps are downloaded to find a mate, make money, or *unplug* —
news must be the third, an escape not a stressor; "demonstrate your core value within the first
three seconds"; night-one friend density decides survival; build apps "that make you feel good
about yourself" (Lenny's Newsletter interview). The reframe pattern: Duolingo moved from XP-grind
to "one lesson a day" and sold identity ("I keep my streak"); Wordle sold *completion* — "one
Wordle means you've completed 100% of something" (Penn/Lamberton) — and scarcity ended the session
for you; Oura collapsed a data firehose into one glanceable number. **Stop asking users to do the
open-ended hard thing; sell a bounded ritual with a clean finish.**

**Why news is the hard job** (Reuters Institute DNR 2024): **39% selectively avoid news** (up from
29% in 2017); 39% feel "worn out" by the volume; stated reasons are anxiety, powerlessness,
repetition. News fails as a job because it is unbounded, negative, and disempowering.

## The ten principles → conformance audit of app-v3

| # | Principle (lens) | In app-v3 | Status |
|---|---|---|---|
| 1 | Optimize for finished trust, not dwell time (Substack) | Finite Stack, exit ritual "Nothing is waiting for you here" | ✅ |
| 2 | The person is the product; follow people not topics (Substack) | Following tiles, creator profiles, Wire bylines; headlines navigate, faces attribute | ✅ |
| 3 | Bounded low-anxiety "inbox" the reader controls (Substack) | 4-story Stack replaces the unread pile; no red dots anywhere | ✅ |
| 4 | Feed = matchmaking, not outrage (Substack) | Wire is chronological in prototype; **rule for the real build: rank for "who will this reader trust and follow," never engagement** | ⚠️ spec note for Brijesh |
| 5 | Daily ritual + finish line news never had (Substack) | Film-countdown in, completion moment out, Edition collected | ✅ |
| 6 | Sell "finished," not "informed" (Bier/Wordle) | "Then you're done for the day" is the promise line; recap = proof | ✅ |
| 7 | Value in three seconds, no ask before the magic (Bier) | Boots straight to Home + Stack card; no walls in prototype; **real build: no signup before first Stack** | ✅ / spec note |
| 8 | Capable, never powerless (Bier, Reuters) | Takeaways ("the 4 things you now know"), untracked quizzes, no wrong-state shaming | ✅ |
| 9 | Ration the firehose; scarcity is the product (Wordle/Oura) | 4 stories is the point; streak + shield; static "tomorrow 7am," no urgency timer | ✅ |
| 10 | Give the ritual a social edge (Bier) | Share artifact, friend presence ("Maya finished today"), The Wire, Activity without badges | ✅ |

Audit conclusion: app-v3 conforms on 9/10; #4 and the #7 signup rule are carried as explicit
requirements into the Brijesh build spec, since the prototype has no ranking or auth to implement.

## North-star check for any future change

Does it make tomorrow's open more likely, the reader feel more capable, or the completion moment
stronger? If none of the three — cut it.
