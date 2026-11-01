# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Users

One user: Alex, the owner of the plants and of the app. H₂Grow is a personal journal for Alex's own collection. It is not built for other plant owners, and nobody else has to be able to use it.

## Product Purpose

H₂Grow keeps the care and growth record of a home plant collection in one place. It succeeds when three jobs, all equally important, feel easy:

- **Know what needs attention.** Opening the app shows which plants are due for a water check today.
- **Log care fast.** Recording a watering, feeding, repot, prune, treatment, growth check-in or note takes seconds, usually on a phone.
- **See growth over time.** Each plant builds a timeline of measurements (height, leaf count), notes and progress photos.

## Positioning

A plant parent's journal, not a care-schedule utility. The app treats each plant as a named individual with its own story ("Olive", "Pepper", "Sol"), and treats every care moment as an entry in that story rather than a ticked-off task.

## Operating Context

- Used mostly on a phone, often installed to the home screen and opened next to the plants, sometimes with spotty connectivity.
- Each plant has a name, species, location, date acquired, watering interval in days, light, pot, soil, notes and an optional photo.
- Care event types: watered, fertilized, repotted, pruned, pest/health treatment, growth check-in, observation. Any event can carry height (inches), leaf count, a note and a photo; an event with measurements or a photo counts as a growth update.
- "Needs attention" means no watering has been logged, or the days since the last watering have reached the plant's interval.

## Capabilities and Constraints

- Current build: plain HTML, CSS and JavaScript (`index.html`, `styles.css`, `script.js`) with no framework or build step.
- Installable PWA (`manifest.webmanifest`, `service-worker.js`) that works offline.
- Data lives only in the device's browser storage (`localStorage` key `frond-plant-journal-v2`). Photos are stored inline as data URLs, so storage can fill up. There are no accounts, no sync and no backend.
- New installs start with three sample plants (Olive, Pepper, Sol).
- Alex has said all of these technical choices can change if a change makes the app better; none is a fixed requirement.
- Open: backup/export, sync across devices, and care reminders are not built and have not been decided.

## Brand Commitments

- Name: **H₂Grow**, written with the subscript ₂ (wordmark "H₂" + "Grow"). The PWA short name is "H₂Grow".
- Personal title: "Alex's Plantas". The collection is called "my plantas", and Spanish-English phrasing is part of the voice.
- Voice: warm, personal and playful, as in "Log a little love.", "my happy place" and "proud plant-parent moment". The copy speaks to Alex directly.
- App icons: `icon-192.png`, `icon-512.png`.

## Evidence on Hand

- The only plant data is the three sample plants in `script.js`. No real photos, usage data or other content is in the repository.
- Since the app is for one person, it needs no testimonials, user counts or marketing claims, and future work should not invent them.

## Product Principles

1. **Built for one.** Design for Alex's own collection and habits, not for a general audience.
2. **Today first, history always.** The day's attention list and the long-term record carry equal weight; neither should hide the other.
3. **Seconds to log.** Recording care on a phone, next to the plant, must stay quick and need little typing.
4. **Every plant is a character.** Names, photos and growth stories matter more than care data presented as a spreadsheet.
5. **Alex's data stays safe.** Never lose history silently, and warn when storage limits threaten it.
