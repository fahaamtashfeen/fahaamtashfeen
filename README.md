# Fahaam Tashfeen

Embedded and full-stack developer. Carleton University, BCS (Software Engineering), 2026.

I've also been making music for 11+ years and have produced for Roddy Ricch, NLE Choppa, Yeat, MMZ, Gary Vaynerchuk and others.

[LinkedIn](https://www.linkedin.com/in/fahaam) · [zenith.gallery](https://zenith.gallery) · [beatdrop.zenith.gallery](https://beatdrop.zenith.gallery)

## Projects

### Naloxone delivery drone
*STM32F407 · FreeRTOS · C · I2C*

A drone designed to deliver naloxone (Narcan) to overdose scenes. Prototype built for a QNX-sponsored RTOS course at Carleton.

- Designed the full schematic, sourced the parts and hand-soldered the electronics, with 3D-printed mounts
- Evaluated QNX first, then moved to FreeRTOS when QNX no longer supported the board
- FreeRTOS task architecture running on the STM32F407
- Brought up the IMU over I2C and caught a counterfeit chip when its WHO_AM_I register returned the wrong ID

**Status:** hardware built and brought up, not flying yet.

<!-- Add a photo of the board here (drag it into GitHub's editor) and a link to the repo once it's public -->

### Zenith Gallery · [zenith.gallery](https://zenith.gallery)
*React · Node/Express · MongoDB · Stripe · AWS · Heroku*

A live storefront for beats, sample packs and drum kits. I built it end to end and run it.

- Stripe payments and webhooks, with purchases delivered through AWS S3 presigned URLs
- Google OAuth and JWT auth, transactional email through AWS SES
- Sentry for error monitoring, PostHog for analytics, DNS on Cloudflare
- Production bugs I tracked down: a duplicate Stripe webhook endpoint, a casing mismatch (PascalCase in MongoDB, kebab-case in the frontend) in S3 presigned download links, and a Heroku H12 timeout on the empty-cart route
- Currently expanding it into a multi-vendor marketplace

The repo is private since the store is live. Happy to walk through the code.

### BeatDrop · [beatdrop.zenith.gallery](https://beatdrop.zenith.gallery)
*SvelteKit · Supabase · Cloudflare Pages · YouTube Data API v3 · Gemini*

YouTube uploader for producers. It turns a beat and cover art into a video, writes the title and tags with Gemini, and publishes through the YouTube Data API. Each user connects their own Google Cloud OAuth client and Gemini key, so their credentials and API quota stay their own.

## Tech

| Area | Skills |
| --- | --- |
| **Languages** | C, C++, JavaScript, Python, Java |
| **Embedded** | STM32, FreeRTOS, RTOS architecture, I2C, schematic design, PCB soldering, hardware bring-up |
| **Web** | React, Node.js, Express, MongoDB, SvelteKit, Supabase, HTML/CSS |
| **Cloud & services** | AWS (S3, SES), Stripe, Heroku, Cloudflare, Sentry, PostHog |
| **Tools** | Git, Linux |
