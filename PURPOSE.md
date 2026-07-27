# Newsreel app — purpose (locked before the v3 redesign)

Researched through the lens of Substack's app designers, Nikita Bier, and builders who made
hard daily jobs feel good (Wordle/NYT Games, Duolingo, Oura, People magazine). Distilled July 26, 2026;
v3 (`app-v3.html`) is built against this.

## The purpose, one sentence

**Re-engage people who have given up on news by making the news finishable: open the app, see in
one glance what today asks of you, do it in ~5 minutes, feel smart, leave knowing you're done —
told by verified humans you recognize.**

## The job to be done

Not "stay informed" (nobody's actual job) but: **"let me feel caught up and smart without feeling
anxious, dumb, or behind."** News apps fail because they make users feel behind and stupid; the feed
never ends, so there is no moment of "done." The product's unit of value is the *completion moment*,
not the impression.

## What each lens contributed

- **Substack designers**: people follow *people*, not outlets. Faces and bylines are the durable
  retention asset. But (Brijesh's corollary) avatar-first navigation only works when the person IS
  the product; in news, headlines must navigate and faces attribute — content-consent before commit.
- **Nikita Bier**: night-one social density decides retention; presence not pressure ("Maya finished
  today," never a nag). Ship the smallest loop that produces a feeling, and let the feeling market it.
- **Wordle / NYT Games**: the daily gate converts completion into anticipation. Push the reward
  screen (recap + streak + next-edition + share on ONE screen). Scarcity is a feature — "won't let
  you binge" is the moat, not a limitation.
- **Duolingo**: ritual chrome (streaks, pips, celebration) works when the metric is showing up, not
  performance. Streak with a shield; no XP on news (grinding mechanics read as cynical here).
- **Oura**: one glance = your state ("readiness 82" → "1/4 done, 3 left"). The home is a status
  surface first, a library second.
- **People magazine**: art direction with clear jobs — image leads, type captions, format is legible
  at a glance. Text-heavy = wrong.

## Structural consequences (all shipped in v3)

1. **Home is the front door** (was the Explore tab's role): greeting, Today's Stack card (filmstrip,
   ring, one CTA), Following tiles, Catch me up (Timeline / Split Screen / Ask Benny), daily question,
   browse mosaic. The swipe feed is no longer the app's opening statement.
2. **The feed is demoted from primary** — reachable from every story tile/hero; tab 2 evolved
   (Feed → Browse → The Wire) per Jack's direction into the social surface: journalists + friends.
3. **The Stack is a passage**: film-countdown in, tabs vanish, chapter cards, three native formats
   (brief / video / article with a "Full story" door), exit ritual ("You're caught up. Nothing is
   waiting for you here.") with recap, streak, share.
4. **Format language**: IG-style glyphs + Substack-style cost units ("5 cards" / "0:58" / "11 min
   read") + paper chrome for articles, applied on every surface.
5. **North-star check for any future change**: does it make tomorrow's open more likely, the user
   feel smarter, or the completion moment stronger? If none — cut it.
