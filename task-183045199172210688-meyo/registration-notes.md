# Registration & Posting Notes — 觅游社区

## What We Know

### 觅游 Community Overview
- Chinese developer/AI community
- Active discussions around AI tools, Agent building, memory systems, cron automation
- Values authentic experience-sharing over promotional content
- Community has "虾" (shrimp) avatar system with karma/points

### Posting Requirements (from task brief)
- Post as an "AI resident" (AI 居民)
- Post content should demonstrate genuine value
- Posting = reward eligibility

### Account Requirements
- **Account**: Need a 觅游 community account (registration URL TBC)
- **Auth method**: Unknown — likely email/phone + password or OAuth
- **Agent posting**: Unknown if API-based posting is supported, or if browser automation required

## What We Still Need

### Critical Questions (Blocking)

| # | Question | Why It Matters |
|---|----------|----------------|
| 1 | What is the 觅游 community URL? | We need to know where to register and post |
| 2 | Is there an API for posting, or must we use the web UI? | Determines whether we can automate posting or need browser-use fallback |
| 3 | Does the account need to be created manually, or can we register via API? | Registration flow affects automation strategy |
| 4 | What are the "发帖即领赏" reward criteria? | We need to ensure the post meets reward eligibility |
| 5 | Is there a minimum account age/karma requirement before posting? | New accounts may have restrictions |

### Nice-to-Know (Non-blocking)

- Community moderation rules (avoid being flagged as spam)
- Optimal posting times for visibility
- Tag/hashtag system for content discovery
- Character limit for posts

## Posting Strategy

### If API available:
1. Register account → authenticate
2. Post draft via API
3. Confirm post is live
4. Update task status to `posted`

### If browser automation required:
1. Use `browser-use` skill to navigate to 觅游
2. Complete registration flow
3. Log in and navigate to post creation
4. Fill in draft content and submit
5. Take screenshot as proof
6. Update task status to `posted`

### Fallback:
If neither API nor browser automation works (e.g., CAPTCHA, phone verification), escalate to requester for manual posting assistance.

## Draft Status

- ✅ Content drafted (post-draft.md) — 300-500 word Chinese post, AI resident perspective
- ⏳ Awaiting: account auth details, posting method confirmation
- ⏳ Awaiting: task brief clarification on reward criteria
