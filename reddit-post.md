# Reddit Post — r/androidapps / r/learnprogramming / r/ifyoulikeblank

**Title:** I built an AI music discovery app that actually gets what I like — here's what I learned about building Songdio

---

Hey everyone 👋

I'm a solo dev who's been working on **Songdio** — an AI-powered music discovery app — and I wanted to share it with this community because honestly, some of the best feedback I've gotten came from posts like this one.

## The Problem

Spotify's algorithm is fine, but it keeps me in a bubble. YouTube's recommendations are great until you end up listening to the same 5 playlists on repeat. I wanted something that *actively introduces* me to music outside my comfort zone — not just more of the same.

So I built Songdio.

## What Songdio Does

At its core, Songdio is a **cross-platform music discovery tool** that combines:

- **AI-powered taste profiling** — You tell it a few artists you love, and it builds a deeper taste model than just "people who liked X also liked Y." It analyzes your listening patterns, mood preferences, and even musical structure.
- **Global music curation** — This is the part I'm most excited about. Songdio surfaces music from international scenes: Japanese city pop, Korean indie, African electronic, Latin alternative — stuff you'd never find in a Western algorithm bubble.
- **Community-driven playlists** — Users create and share discovery playlists. Think of it like a crowdsourced radio station that evolves over time.
- **Seamless cross-device** — Start on your phone, continue on your laptop. No friction.

## The Tech Stack (for the devs in here)

Since this is partly a dev community, here's the stack:

- **Frontend:** React Native (cross-platform iOS/Android)
- **Backend:** FastAPI + PostgreSQL
- **AI/ML:** Custom taste-modeling pipeline using collaborative filtering + content-based analysis. I'm using a fine-tuned model that learns from listening behavior, not just metadata.
- **Audio Analysis:** Librosa for feature extraction (tempo, energy, spectral characteristics)
- **Infrastructure:** Docker on AWS, with Redis for caching and Celery for async tasks

The most interesting technical challenge was building the "taste bridge" algorithm — how do you connect a user who likes Tame Impala to someone who might enjoy Khruangbin without it feeling random? That's where the content-based audio analysis really shines.

## What I've Learned

A few things from building this over the past 6 months:

1. **Music taste is more contextual than you think.** People don't just like genres — they like *vibes*. A song that's perfect for a workout is different from one that's perfect for studying. Songdio's mood-aware recommendations try to capture that.

2. **International music is underserved.** There's incredible music being made everywhere, but discovery tools are overwhelmingly Western-centric. Building Songdio's global curation pipeline was hard but incredibly rewarding.

3. **Community is everything.** The best features in Songdio came from user feedback. The playlist sharing, the taste profile sharing, the "surprise me" mode — all user suggestions.

## Try It Out

If this sounds interesting, I'd love for you to check it out:

🌐 **Website:** [songdio.com](https://songdio.com)
📱 **iOS:** [App Store](https://apps.apple.com/songdio)
🤖 **Android:** [Google Play](https://play.google.com/songdio)

I'm offering **free premium access for 3 months** to anyone who signs up from this post — just use code **REDDITFAM** at checkout.

## Feedback Welcome

I'm actively developing this and your feedback directly shapes the roadmap. Whether it's bug reports, feature requests, or just "hey this is cool" — I'm all ears.

Drop a comment below or DM me. Happy to chat about the tech, the music curation philosophy, or just share some good music recs. 🎵

---

*Edit: Wow, this blew up way more than I expected. Thanks for all the love, everyone! I'm going through every single comment. If I haven't replied to you yet, I will — just give me a bit. Also, the code REDDITFAM has been extended for another week for anyone who missed it.*
