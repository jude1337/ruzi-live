<img width="1892" height="941" alt="landing" src="[https://raw.githubusercontent.com/jude1337/ruzi-live/refs/heads/main/ruzi-live-landing.png" />

<p align="center">
  <a href="https://ruzi.live/">
    <h1 align="center">ruzi.live</h1>
  </a>
</p>

<p align="center">
Official site for Twitch streamer <strong>Ruzi (13ruzi)</strong> featuring live embeds, awards voting, arcade games, and community pages.
</p>
<br/>

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#introduction">Intro</a></li>
    <li><a href="#techstack">Techstack</a></li>
    <li><a href="#features-technical">Features</a></li>
    <li><a href="#project-structure">Project Structure</a></li>
  </ol>
</details>

<hr />

## Introduction

This repo contains the full codebase for ruzi.live, built to showcase Ruzi’s stream, community events, and interactive features. It includes Twitch OAuth, awards voting (phase 1/phase 2), admin tooling, and a Ruzi Runner arcade game with a persistent leaderboard.

## Techstack

- Next.js 15 (App Router)
- TypeScript
- Tailwind CSS + shadcn-style UI primitives
- Framer Motion animations
- MySQL/MariaDB via `mysql2`
- Pusher (live alerts / realtime updates)
- Twitch OAuth + Helix API integrations

## Features

- Twitch live stream page with chat embed controls
- Clips browser with Twitch API
- Ruzi Runner arcade game + leaderboard + Ruzees rewards
- Casino mini-games (slots, blackjack, roulette)
- Awards voting (phase 1 typed submissions, phase 2 preset picks)
- Vote results dashboards + CSV export
- Awards reveal show page for stream overlays
- Twitch overlay alerts for redemptions
- Admin dashboard: bans, balances, leaderboard edits, vote results, SMP announcements
- RuziSMP status + announcements + player list
- Gallery page auto-loading media from `public/gallery`
- Auth gating for admin + results pages

## Project Structure

```
├── src
│   ├── app
│   │   ├── admin
│   │   ├── api
│   │   ├── clips
│   │   ├── gallery
│   │   ├── games
│   │   ├── live
│   │   ├── og
│   │   ├── overlay
│   │   ├── ruzismp
│   │   ├── vote
│   │   └── ...
│   ├── components
│   ├── data
│   ├── lib
│   └── styles
├── public
├── data
└── ...
```
