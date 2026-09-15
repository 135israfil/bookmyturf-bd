# BookMyTurf BD

A sports turf booking platform for the Bangladesh market, with a planned mobile app build sequenced to ship a working product fast and rebuild natively only once that's proven.

**Status:** web platform live; mobile build planned in detail. Source is private; this repo documents the platform and the mobile build plan.

## Why I built this

Turf booking in Bangladesh is still largely phone calls and word of mouth. BookMyTurf BD digitizes that — real-time availability, booking, and payment for sports turfs — on a stack chosen to ship fast on the web first, with mobile planned as a deliberate second phase rather than built in parallel from day one.

## What it does

- Real-time turf availability and booking for the Bangladesh market
- A phased mobile strategy: a Capacitor webview MVP first (wrapping the existing web app to get to app stores fast and validate demand), then a native React Native or Flutter rebuild once the product is proven — rather than committing to native development before knowing the app is worth the investment
- Client-facing project quotations and store-readiness documentation produced as part of scoping the mobile phase

## Architecture

Next.js on the frontend, Prisma as the ORM, Supabase as the backend/database layer — a stack chosen for speed of iteration on a platform serving a regional market where the priority is proving the product works before over-investing in infrastructure.

## Stack

Next.js, Prisma, Supabase.

## What I'd do differently

The Capacitor-first, native-second sequencing is the right call here and I'd keep it — but I'd define the specific metric that triggers the native rebuild (a usage threshold, a specific complaint pattern about webview performance) up front, rather than leaving "once it's proven" as a judgment call to be made later without a pre-agreed bar.
