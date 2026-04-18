<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Module 32 - The Snapchat Playbook | The Creator Plug Academy</title>
  <style>
    :root {
      --ink: #24192f;
      --muted: #6f6178;
      --panel: #ffffff;
      --gold: #d9a441;
      --gold-soft: #fff2c9;
      --rose: #f05d8a;
      --teal: #18a6a7;
      --violet: #4d2770;
      --violet-deep: #241332;
      --line: #eadfce;
      --shadow: 0 18px 40px rgba(48, 31, 61, 0.14);
    }
    * { box-sizing: border-box; }
    html { scroll-behavior: smooth; }
    body {
      margin: 0;
      font-family: Arial, Helvetica, sans-serif;
      color: var(--ink);
      background:
        radial-gradient(circle at 14% 8%, rgba(240, 93, 138, 0.15), transparent 28%),
        radial-gradient(circle at 88% 4%, rgba(24, 166, 167, 0.16), transparent 26%),
        linear-gradient(180deg, #fffaf1 0%, #f8f1e7 45%, #f4ebdd 100%);
      line-height: 1.6;
    }
    a { color: #2c6f91; font-weight: 800; }
    .page { width: min(1120px, calc(100% - 32px)); margin: 0 auto; padding: 28px 0 56px; }
    .hero { background: linear-gradient(135deg, rgba(36, 19, 50, 0.96), rgba(77, 39, 112, 0.92)); color: #fff; border-radius: 8px; padding: 34px; box-shadow: var(--shadow); position: relative; overflow: hidden; }
    .hero:after { content: ""; position: absolute; right: -78px; top: -82px; width: 260px; height: 260px; border: 2px solid rgba(217, 164, 65, 0.36); transform: rotate(20deg); }
    .eyebrow { display: inline-flex; background: rgba(217, 164, 65, 0.18); border: 1px solid rgba(217, 164, 65, 0.45); color: #ffe3a0; border-radius: 8px; padding: 7px 11px; font-size: 13px; font-weight: 800; letter-spacing: 0.08em; text-transform: uppercase; }
    h1, h2, h3 { line-height: 1.15; margin: 0; }
    h1 { max-width: 900px; margin-top: 18px; font-size: clamp(34px, 6vw, 70px); }
    .subtitle { max-width: 880px; margin: 18px 0 0; color: #f6e9d6; font-size: 18px; }
    .quick-links { display: flex; flex-wrap: wrap; gap: 10px; margin-top: 24px; position: relative; z-index: 1; }
    .quick-links a, .copy-button { appearance: none; border: 0; border-radius: 8px; background: var(--gold); color: #241332; cursor: pointer; display: inline-flex; align-items: center; justify-content: center; font-family: inherit; font-size: 14px; font-weight: 900; line-height: 1; min-height: 42px; padding: 12px 14px; text-decoration: none; }
    .quick-links a:hover, .copy-button:hover { background: #f1c761; }
    .hero-grid, .three-col { display: grid; grid-template-columns: repeat(3, 1fr); gap: 14px; margin-top: 26px; }
    .hero-card { background: rgba(255, 255, 255, 0.1); border: 1px solid rgba(255, 255, 255, 0.18); border-radius: 8px; padding: 18px; min-height: 126px; }
    .hero-card strong { color: #ffe1a1; display: block; font-size: 15px; text-transform: uppercase; letter-spacing: 0.08em; margin-bottom: 8px; }
    .section { margin-top: 24px; background: rgba(255, 255, 255, 0.88); border: 1px solid var(--line); border-radius: 8px; padding: 28px; box-shadow: 0 10px 24px rgba(48, 31, 61, 0.08); }
    .section h2 { color: var(--violet-deep); font-size: clamp(25px, 3vw, 38px); margin-bottom: 12px; }
    .section-intro { max-width: 900px; color: var(--muted); margin: 0 0 20px; }
    .two-col { display: grid; grid-template-columns: repeat(2, 1fr); gap: 16px; }
    .card { background: var(--panel); border: 1px solid var(--line); border-radius: 8px; padding: 20px; }
    .card h3 { color: var(--violet); font-size: 20px; margin-bottom: 8px; }
    .tag { display: inline-block; border-radius: 8px; padding: 5px 9px; margin-bottom: 12px; background: var(--gold-soft); color: #765210; font-weight: 800; font-size: 12px; text-transform: uppercase; letter-spacing: 0.06em; }
    ul, ol { margin: 10px 0 0 20px; padding: 0; }
    li { margin: 8px 0; }
    .link-grid { display: grid; grid-template-columns: repeat(2, 1fr); gap: 12px; margin-bottom: 24px; }
    .lesson-link { background: #fff; border: 1px solid var(--line); border-radius: 8px; color: var(--violet-deep); display: block; font-weight: 800; padding: 14px; text-decoration: none; }
    .lesson-link:hover { border-color: var(--gold); box-shadow: 0 8px 20px rgba(48, 31, 61, 0.1); transform: translateY(-1px); }
    .lesson { display: grid; grid-template-columns: 84px 1fr; gap: 16px; border-top: 1px solid var(--line); padding: 20px 0; }
    .lesson:first-of-type { border-top: 0; padding-top: 0; }
    .lesson-number { width: 64px; height: 64px; border-radius: 8px; background: linear-gradient(135deg, var(--violet), var(--rose)); color: #fff; display: grid; place-items: center; font-size: 24px; font-weight: 900; box-shadow: 0 12px 22px rgba(77, 39, 112, 0.22); }
    .lesson-number a { color: #fff; display: grid; height: 100%; place-items: center; text-decoration: none; width: 100%; }
    .callout { border-left: 5px solid var(--gold); background: #fff7dc; padding: 16px 18px; border-radius: 8px; margin-top: 16px; }
    .warning { border-left-color: var(--rose); background: #fff0f5; }
    table { width: 100%; border-collapse: collapse; overflow: hidden; border-radius: 8px; background: #fff; border: 1px solid var(--line); margin-top: 14px; }
    th, td { text-align: left; vertical-align: top; border-bottom: 1px solid var(--line); padding: 14px; }
    th { background: var(--violet-deep); color: #fff; font-size: 13px; text-transform: uppercase; letter-spacing: 0.06em; }
    tr:last-child td { border-bottom: 0; }
    .script-box { background: #241332; color: #fdf5e8; border-radius: 8px; padding: 18px; font-family: "Courier New", Courier, monospace; font-size: 14px; line-height: 1.55; white-space: pre-wrap; }
    .copy-row { align-items: center; display: flex; flex-wrap: wrap; gap: 10px; justify-content: space-between; margin-bottom: 10px; }
    .checklist { list-style: none; margin-left: 0; }
    .checklist li { padding-left: 34px; position: relative; }
    .checklist li:before { content: ""; position: absolute; left: 0; top: 5px; width: 19px; height: 19px; border-radius: 5px; border: 2px solid var(--teal); background: #efffff; }
    .footer { margin-top: 24px; text-align: center; color: var(--muted); font-size: 14px; }
    @media (max-width: 820px) {
      .hero { padding: 24px; }
      .hero-grid, .two-col, .three-col, .link-grid { grid-template-columns: 1fr; }
      .lesson { grid-template-columns: 1fr; }
      table, thead, tbody, th, td, tr { display: block; }
      th { display: none; }
    }
  </style>
</head>
<body>
  <main class="page">
    <section class="hero">
      <span class="eyebrow">Module 32</span>
      <h1>The Snapchat Playbook</h1>
      <p class="subtitle">Build an audience and income on Snapchat's creator platform through Spotlight, Stories, Creator Profiles, AR Lenses, brand partnerships, subscriptions, and Snap's unified monetization system.</p>
      <nav class="quick-links" aria-label="Quick links">
        <a href="#lessons">Lessons</a>
        <a href="#launch-plan">30-Day Plan</a>
        <a href="#copy-tools">Copy Tools</a>
        <a href="#resources">Resource Links</a>
      </nav>
      <div class="hero-grid">
        <div class="hero-card"><strong>Platform Edge</strong>Snap is less crowded than TikTok and Instagram for many creators, while still having massive daily creator consumption.</div>
        <div class="hero-card"><strong>Core Channels</strong>Creator Profiles, Public Stories, Spotlight, Lens Studio, Creator Marketplace, and paid subscriptions.</div>
        <div class="hero-card"><strong>2026 Update</strong>Snap's old standalone Spotlight Rewards ended in 2025. Monetization now centers on the unified Monetization Program and Creator Rewards.</div>
      </div>
    </section>

    <section class="section" id="welcome">
      <h2>Welcome to Module 32</h2>
      <p class="section-intro">Snapchat is no longer just disappearing selfies. It is a content and creator ecosystem with Spotlight, Public Stories, AR, creator profiles, monetization tools, and a daily audience that values authenticity.</p>
      <div class="callout">Accuracy note: Snap announced 946 million monthly active users in Q4 2025 and launched Creator Subscriptions alpha testing in February 2026. This page updates the older "Spotlight bonus" language to match the unified Monetization Program.</div>
    </section>

    <section class="section" id="lessons">
      <h2>Lessons</h2>
      <div class="link-grid">
        <a class="lesson-link" href="#lesson-1">1. Snapchat in 2026</a>
        <a class="lesson-link" href="#lesson-2">2. Creator features</a>
        <a class="lesson-link" href="#lesson-3">3. Creator profile setup</a>
        <a class="lesson-link" href="#lesson-4">4. Content strategy</a>
        <a class="lesson-link" href="#lesson-5">5. Spotlight strategy</a>
        <a class="lesson-link" href="#lesson-6">6. Stories loyalty</a>
        <a class="lesson-link" href="#lesson-7">7. AR Lenses</a>
        <a class="lesson-link" href="#lesson-8">8. Monetization options</a>
        <a class="lesson-link" href="#lesson-9">9. Cross-platform strategy</a>
        <a class="lesson-link" href="#lesson-10">10. Niche playbooks</a>
        <a class="lesson-link" href="#lesson-11">11. Analytics</a>
        <a class="lesson-link" href="#lesson-12">12. Business and brand building</a>
        <a class="lesson-link" href="#lesson-13">13. Rules and guidelines</a>
        <a class="lesson-link" href="#launch-plan">14. 30-Day launch plan</a>
      </div>

      <article class="lesson" id="lesson-1">
        <div class="lesson-number"><a href="#lesson-1">1</a></div>
        <div>
          <h3>Snapchat in 2026: What Most Creators Don't Know</h3>
          <p>Snapchat was underestimated while creators crowded onto TikTok and Instagram. Snap kept building: Public Profiles, Spotlight, AR, monetization tools, subscriptions, and brand partnership pathways.</p>
          <div class="two-col">
            <div class="card"><h3>Audience</h3><p>Snap reported 946 million monthly active users in Q4 2025, with strong Gen Z and Millennial usage.</p></div>
            <div class="card"><h3>Creative Style</h3><p>Less polished content often feels more natural on Snap. Raw, quick, intimate, and daily wins.</p></div>
            <div class="card"><h3>AR Advantage</h3><p>Snap remains a leader in AR Lenses and creator-built camera experiences.</p></div>
            <div class="card"><h3>Less Crowded</h3><p>Many creators still treat Snap as secondary, which leaves room for consistent niche builders.</p></div>
          </div>
        </div>
      </article>

      <article class="lesson" id="lesson-2">
        <div class="lesson-number"><a href="#lesson-2">2</a></div>
        <div>
          <h3>Understanding Snapchat's Creator Features</h3>
          <table>
            <thead><tr><th>Feature</th><th>Purpose</th></tr></thead>
            <tbody>
              <tr><td>Public Stories</td><td>Daily loyalty content that sits on your public creator profile.</td></tr>
              <tr><td>Spotlight</td><td>Discovery feed for vertical video and viral reach.</td></tr>
              <tr><td>Creator Profile</td><td>Your public hub with Stories, Spotlight videos, subscribers, and profile info.</td></tr>
              <tr><td>Lens Studio</td><td>Snap's free AR creation tool for Lenses, effects, games, and branded experiences.</td></tr>
              <tr><td>Creator Subscriptions</td><td>Premium content layer for eligible creators, launched in alpha in 2026.</td></tr>
              <tr><td>Creator Marketplace / Collab Studio</td><td>Brand discovery and creator partnership pathways.</td></tr>
            </tbody>
          </table>
        </div>
      </article>

      <article class="lesson" id="lesson-3">
        <div class="lesson-number"><a href="#lesson-3">3</a></div>
        <div>
          <h3>Setting Up Your Snapchat Creator Profile</h3>
          <ol>
            <li>Create or update your Snapchat account.</li>
            <li>Create a Public Profile or Creator Profile if eligible.</li>
            <li>Choose a username consistent with your brand.</li>
            <li>Use a recognizable photo or Bitmoji.</li>
            <li>Write a clear bio with niche, value, and reason to subscribe.</li>
            <li>Link your other platforms where available.</li>
            <li>Select your category and turn on eligible creator features.</li>
          </ol>
          <div class="callout">Your profile should answer three questions fast: who are you, what do you post, and why should someone subscribe today?</div>
        </div>
      </article>

      <article class="lesson" id="lesson-4">
        <div class="lesson-number"><a href="#lesson-4">4</a></div>
        <div>
          <h3>Content Strategy for Snapchat</h3>
          <p>Snap rewards immediacy. Think fast hook, raw delivery, full-screen vertical video, text overlays, and strong emotion.</p>
          <table>
            <thead><tr><th>Format</th><th>What Works</th></tr></thead>
            <tbody>
              <tr><td>Spotlight</td><td>Strong 1-2 second hook, vertical video, trending sounds, captions, relatable moment, strong reaction.</td></tr>
              <tr><td>Stories</td><td>Behind the scenes, daily sequences, real-time updates, polls, questions, product reveals, personality.</td></tr>
              <tr><td>Best niches</td><td>Humor, entertainment, sports reactions, beauty, food, relationships, culture, faith, motivation, business.</td></tr>
            </tbody>
          </table>
          <div class="script-box">Strong hook (0-2 sec) + Value or entertainment + Engagement trigger</div>
        </div>
      </article>

      <article class="lesson" id="lesson-5">
        <div class="lesson-number"><a href="#lesson-5">5</a></div>
        <div>
          <h3>Snapchat Spotlight: How to Grow and Monetize</h3>
          <p>Spotlight is still key for discovery, but the old standalone Spotlight Rewards Program ended on January 31, 2025. Snap now points creators toward its unified Monetization Program, which can include monetization for eligible Stories and longer Spotlight videos.</p>
          <h4>Current unified program basics from Snap's 2024 announcement</h4>
          <ul>
            <li>Potential invitation requires at least 50,000 followers.</li>
            <li>Creators should post at least 25 times per month to Saved Stories or Spotlight.</li>
            <li>Creators should post on at least 10 of the last 28 days.</li>
            <li>Creators need one of these in the last 28 days: 10 million Snap views, 1 million Spotlight views, or 12,000 hours of view time.</li>
          </ul>
          <h4>Spotlight performance strategy</h4>
          <ul>
            <li>Post 3-5 videos per day during growth sprints.</li>
            <li>Use Snap's licensed sounds and native tools.</li>
            <li>Remove third-party watermarks before crossposting.</li>
            <li>Reverse-engineer your best hooks, lengths, topics, and posting windows.</li>
          </ul>
        </div>
      </article>

      <article class="lesson" id="lesson-6">
        <div class="lesson-number"><a href="#lesson-6">6</a></div>
        <div>
          <h3>Snapchat Stories: Building Loyal Daily Viewers</h3>
          <p>Spotlight drives discovery. Stories build relationship. The goal is to create a daily check-in habit.</p>
          <div class="two-col">
            <div class="card"><h3>Daily Check-ins</h3><p>Morning updates, what you are working on, and real-time behind the scenes.</p></div>
            <div class="card"><h3>Ongoing Narratives</h3><p>Document a project, goal, challenge, transformation, or launch over multiple days.</p></div>
            <div class="card"><h3>Interactive Tools</h3><p>Polls, question boxes, links, countdowns, music, text overlays, and drawings.</p></div>
            <div class="card"><h3>Subscriber Content</h3><p>For eligible creators, use subscriptions for deeper, more personal, premium Stories.</p></div>
          </div>
        </div>
      </article>

      <article class="lesson" id="lesson-7">
        <div class="lesson-number"><a href="#lesson-7">7</a></div>
        <div>
          <h3>AR Lenses: Your Secret Growth Tool</h3>
          <p>Many creators skip Lens Studio, but Lenses can create brand reach at scale because users spread the Lens for you.</p>
          <ol>
            <li>Use Lens Studio's templates before building from scratch.</li>
            <li>Create a Lens tied to your niche, aesthetic, brand, event, or challenge.</li>
            <li>Submit it for review.</li>
            <li>Promote it in Stories and Spotlight.</li>
            <li>Watch profile taps and usage for growth signals.</li>
          </ol>
        </div>
      </article>

      <article class="lesson" id="lesson-8">
        <div class="lesson-number"><a href="#lesson-8">8</a></div>
        <div>
          <h3>Monetization Options on Snapchat</h3>
          <table>
            <thead><tr><th>Stream</th><th>How It Works</th></tr></thead>
            <tbody>
              <tr><td>Unified Monetization Program</td><td>Eligible invited creators can earn from ads in Stories and longer Spotlight videos.</td></tr>
              <tr><td>Creator Rewards</td><td>Eligible creators can receive rewards for qualifying activity and cash out through Snap's payout system.</td></tr>
              <tr><td>Creator Subscriptions</td><td>Premium Stories, replies, Chat access, and exclusive content for eligible creators.</td></tr>
              <tr><td>Brand deals</td><td>Sponsored Snaps, Stories, Spotlight content, AR campaigns, and native product integrations.</td></tr>
              <tr><td>Off-platform sales</td><td>Use link stickers and CTAs to drive email signups, products, YouTube, Gumroad, Etsy, or Stan Store.</td></tr>
              <tr><td>Creator Marketplace / Collab Studio</td><td>Opt in to brand discovery and partnership opportunities through Snap's creator tools.</td></tr>
            </tbody>
          </table>
          <div class="callout warning">Snap says it does not charge fees or accept payment in exchange for Monetization Program invitations. Treat any third party selling access as a red flag.</div>
        </div>
      </article>

      <article class="lesson" id="lesson-9">
        <div class="lesson-number"><a href="#lesson-9">9</a></div>
        <div>
          <h3>Cross-Platform Strategy: Snapchat + Your Main Platform</h3>
          <p>Snap works best when it has a job inside your larger creator ecosystem.</p>
          <div class="script-box">Viral Spotlight -> Subscribe CTA -> Daily Stories -> Link sticker -> Email list or main platform -> Product sale</div>
          <div class="two-col">
            <div class="card"><h3>Discovery Layer</h3><p>Use Spotlight to reach new people, then direct them to your profile, Stories, YouTube, Instagram, or email list.</p></div>
            <div class="card"><h3>Inner Circle Layer</h3><p>Use Stories for your most personal, casual, daily content so fans feel closer to you.</p></div>
            <div class="card"><h3>Repurpose In</h3><p>Remove watermarks from TikTok/Reels before posting to Spotlight.</p></div>
            <div class="card"><h3>Repurpose Out</h3><p>Turn winning Snap ideas into TikToks, Reels, Shorts, emails, or YouTube concepts.</p></div>
          </div>
        </div>
      </article>

      <article class="lesson" id="lesson-10">
        <div class="lesson-number"><a href="#lesson-10">10</a></div>
        <div>
          <h3>Snapchat for Specific Creator Niches</h3>
          <table>
            <thead><tr><th>Niche</th><th>Snap Playbook</th></tr></thead>
            <tbody>
              <tr><td>Humor and comedy</td><td>Short punchy videos, relatable bits, memes, reactions, volume posting.</td></tr>
              <tr><td>Beauty and fashion</td><td>GRWM, outfit checks, product hauls, day-by-day routines, raw try-ons.</td></tr>
              <tr><td>Food</td><td>Recipe reveals, cooking process, restaurant visits, food hauls, final result first.</td></tr>
              <tr><td>Sports and entertainment</td><td>Live reactions, predictions, hot takes, post-game opinions, event-timed content.</td></tr>
              <tr><td>Faith and motivation</td><td>Morning encouragement, Scripture, testimony, mindset clips, evening reflection.</td></tr>
              <tr><td>Business and finance</td><td>Money tips, founder life, what nobody tells you, daily business lessons.</td></tr>
              <tr><td>Relationships</td><td>Polls, questions, advice, couple content, dating debates, story-driven replies.</td></tr>
              <tr><td>Culture creators</td><td>Community humor, commentary, representation, local language, shared experience.</td></tr>
            </tbody>
          </table>
        </div>
      </article>

      <article class="lesson" id="lesson-11">
        <div class="lesson-number"><a href="#lesson-11">11</a></div>
        <div>
          <h3>Analytics and Growing on Snapchat</h3>
          <p>Snapchat Insights help you understand what earns attention, subscriptions, shares, and monetization eligibility progress.</p>
          <table>
            <thead><tr><th>Metric</th><th>What It Tells You</th></tr></thead>
            <tbody>
              <tr><td>Spotlight views</td><td>Total discovery reach.</td></tr>
              <tr><td>Story views</td><td>Core audience loyalty and daily demand.</td></tr>
              <tr><td>Subscriber growth</td><td>Whether profile CTAs and content promise are working.</td></tr>
              <tr><td>Completion rate</td><td>Whether people finish the Snap.</td></tr>
              <tr><td>Screenshots</td><td>High-value save signal.</td></tr>
              <tr><td>Shares</td><td>Viral potential and social proof.</td></tr>
            </tbody>
          </table>
          <h4>Reverse-engineer wins</h4>
          <ul>
            <li>What was the hook?</li>
            <li>What time was it posted?</li>
            <li>What sound or format was used?</li>
            <li>How long was it?</li>
            <li>What emotion did it trigger?</li>
          </ul>
        </div>
      </article>

      <article class="lesson" id="lesson-12">
        <div class="lesson-number"><a href="#lesson-12">12</a></div>
        <div>
          <h3>Snapchat for Business and Brand Building</h3>
          <div class="two-col">
            <div class="card"><h3>Local Businesses</h3><p>Use public profile, behind-the-scenes, Snap Map-relevant content, and local promotions.</p></div>
            <div class="card"><h3>E-commerce Brands</h3><p>Show products in action, product drops, customer reactions, and link sticker traffic.</p></div>
            <div class="card"><h3>Service Providers</h3><p>Build trust through process videos, client testimonials, day-in-the-life content, and FAQs.</p></div>
            <div class="card"><h3>Personal Brands</h3><p>Use Snap for the human side while other platforms carry the polished authority side.</p></div>
          </div>
        </div>
      </article>

      <article class="lesson" id="lesson-13">
        <div class="lesson-number"><a href="#lesson-13">13</a></div>
        <div>
          <h3>Snapchat Best Practices, Rules, and Community Guidelines</h3>
          <p>Protect the account. Follow Snap's Community Guidelines, music rules, paid partnership requirements, and FTC disclosure rules.</p>
          <div class="two-col">
            <div class="card"><h3>Avoid</h3><p>Graphic violence, nudity, harassment, misinformation, copyright violations, spam posting, fake engagement.</p></div>
            <div class="card"><h3>Protect</h3><p>Use a strong password, two-factor authentication, no credential sharing, and no shady third-party apps.</p></div>
            <div class="card"><h3>Copyright</h3><p>Use Snap's licensed music library and avoid pirated audio, TV/movie clips, and sports footage without rights.</p></div>
            <div class="card"><h3>Disclosure</h3><p>Use paid partnership tools and clear language such as "ad" or "sponsored" where required.</p></div>
          </div>
        </div>
      </article>
    </section>

    <section class="section" id="launch-plan">
      <h2>Lesson 14: Your 30-Day Snapchat Launch Plan</h2>
      <div class="three-col">
        <div class="card">
          <span class="tag">Week 1</span>
          <h3>Set Up and Learn</h3>
          <ul>
            <li>Day 1: Create or update your Creator Profile.</li>
            <li>Day 2: Choose your niche, username, and bio promise.</li>
            <li>Day 3: Post your first 3 Spotlight videos.</li>
            <li>Day 4: Set up Public Story and post 5 Story frames.</li>
            <li>Day 5: Explore Lens Studio templates.</li>
            <li>Day 6-7: Post 3 more Spotlights and check Insights.</li>
          </ul>
        </div>
        <div class="card">
          <span class="tag">Week 2</span>
          <h3>Build the Habit</h3>
          <ul>
            <li>Post 5 Spotlight videos per day for two days.</li>
            <li>Add a link sticker pointing to your main platform.</li>
            <li>Post a poll or question box Story.</li>
            <li>Promote Snap on Instagram, TikTok, or YouTube.</li>
            <li>Test a trending sound.</li>
            <li>Review analytics and double down on the best format.</li>
          </ul>
        </div>
        <div class="card">
          <span class="tag">Weeks 3-4</span>
          <h3>Monetize and Scale</h3>
          <ul>
            <li>Review eligibility for Snap's Monetization Program.</li>
            <li>Enable subscriptions if eligible.</li>
            <li>Opt into brand partnership discovery if available.</li>
            <li>Draft and send a brand pitch.</li>
            <li>Create more of your top 3 Spotlight formats.</li>
            <li>Plan Month 2 posting, collaboration, and income goals.</li>
          </ul>
        </div>
      </div>
    </section>

    <section class="section" id="copy-tools">
      <h2>Copy Tools</h2>
      <p class="section-intro">Use these to speed up your profile, Spotlight hooks, and brand pitches.</p>
      <div class="copy-row">
        <h3>Snap Bio Formula</h3>
        <button class="copy-button" data-copy="bio">Copy</button>
      </div>
      <div class="script-box" id="bio">I help [audience] with [result/topic] through real, daily Snap content.
Subscribe for [specific content promise].
[CTA: follow my Stories / watch Spotlight / grab the link]</div>

      <div class="copy-row" style="margin-top: 18px;">
        <h3>Spotlight Hook Bank</h3>
        <button class="copy-button" data-copy="hooks">Copy</button>
      </div>
      <div class="script-box" id="hooks">Nobody tells you this about [topic]...
Watch what happens when I [action]...
If you are [audience], stop scrolling.
I tried [thing] so you do not have to.
This is your sign to [action].
The fastest way to [result] is...</div>

      <div class="copy-row" style="margin-top: 18px;">
        <h3>Brand Pitch</h3>
        <button class="copy-button" data-copy="pitch">Copy</button>
      </div>
      <div class="script-box" id="pitch">Hi [Brand],

I create Snapchat content for [audience/niche], with a focus on [content style]. I think your [product/service] would fit naturally into my Stories and Spotlight content because [reason].

I can create:
- [deliverable 1]
- [deliverable 2]
- [deliverable 3]

Happy to send my current Snap stats and a quick concept if you are open to collaborating.</div>
    </section>

    <section class="section" id="checklist">
      <h2>Quick Reference: Snapchat Creator Checklist</h2>
      <div class="two-col">
        <div class="card">
          <h3>Profile</h3>
          <ul class="checklist">
            <li>Creator/Public Profile set up.</li>
            <li>Bio clear with niche and CTA.</li>
            <li>Other platforms linked where available.</li>
            <li>Subscriptions enabled if eligible.</li>
          </ul>
        </div>
        <div class="card">
          <h3>Content</h3>
          <ul class="checklist">
            <li>Posting 3-5 Spotlights per day during growth sprint.</li>
            <li>Posting to Stories daily.</li>
            <li>Using Snap's licensed music and native tools.</li>
            <li>Testing hooks and first-frame formats.</li>
          </ul>
        </div>
        <div class="card">
          <h3>Monetization</h3>
          <ul class="checklist">
            <li>Unified Monetization Program eligibility reviewed.</li>
            <li>Creator Rewards Hub understood.</li>
            <li>Brand partnership toggle or marketplace profile reviewed.</li>
            <li>Link stickers used to drive products/platforms.</li>
          </ul>
        </div>
        <div class="card">
          <h3>Growth</h3>
          <ul class="checklist">
            <li>Snap profile promoted elsewhere.</li>
            <li>Analytics reviewed weekly.</li>
            <li>Top formats identified and repeated.</li>
            <li>Brand pitches or collaborations in progress.</li>
          </ul>
        </div>
      </div>
    </section>

    <section class="section" id="resources">
      <h2>Official Resource Links</h2>
      <p class="section-intro">Snap's creator programs change often. Use these current official links before making eligibility or income claims.</p>
      <div class="link-grid">
        <a class="lesson-link" href="https://creators.snapchat.com/content-partners-spotlight" target="_blank" rel="noopener">Snapchat Creator Hub</a>
        <a class="lesson-link" href="https://help.snapchat.com/hc/articles/14669003687444" target="_blank" rel="noopener">Snapchat Monetization Program</a>
        <a class="lesson-link" href="https://help.snapchat.com/hc/en-us/articles/5909152630420-Creator-Rewards-FAQ" target="_blank" rel="noopener">Creator Rewards FAQ</a>
        <a class="lesson-link" href="https://help.snapchat.com/hc/en-us/articles/7012310905876-How-does-Snapchat-determine-who-is-eligible-to-participate-in-the-Spotlight-Reward-Program" target="_blank" rel="noopener">Spotlight Rewards deprecation FAQ</a>
        <a class="lesson-link" href="https://help.snapchat.com/hc/en-us/articles/7012330991124-How-do-I-create-Lenses-for-Snapchat-" target="_blank" rel="noopener">Snapchat Lens Studio help</a>
        <a class="lesson-link" href="https://values.snap.com/privacy/transparency/community-guidelines" target="_blank" rel="noopener">Snap Community Guidelines</a>
        <a class="lesson-link" href="https://www.ftc.gov/influencers" target="_blank" rel="noopener">FTC Influencer Disclosures</a>
        <a class="lesson-link" href="https://newsroom.snap.com/snapchat-launches-creator-subscriptions" target="_blank" rel="noopener">Snap Creator Subscriptions announcement</a>
      </div>
      <div class="callout warning">The standalone Spotlight Rewards Program ended on January 31, 2025. In 2026, creators should check Snap's unified Monetization Program, Creator Rewards Hub, Creator Subscriptions, and brand partnership tools for current eligibility.</div>
    </section>

    <p class="footer">Module 32 - The Creator Plug Academy | Next: Module 33 - Amazon Beyond KDP</p>
  </main>

  <script>
    document.querySelectorAll("[data-copy]").forEach((button) => {
      button.addEventListener("click", async () => {
        const target = document.getElementById(button.dataset.copy);
        if (!target) return;
        await navigator.clipboard.writeText(target.innerText);
        const original = button.innerText;
        button.innerText = "Copied";
        setTimeout(() => { button.innerText = original; }, 1400);
      });
    });
  </script>
</body>
</html>
