# NCSA SPIN Research: mHealth for Cancer Survivors

Undergraduate research through the NCSA Students Pushing Innovation (SPIN) program at the University of Illinois Urbana-Champaign, with the Info Access Lab, advised by Prof. Rachel Adler. August 2026 to present.

> This repository is a public overview of my work. The source code lives in the lab's private repository, and everything described here uses synthetic data.

## The problem

Life after cancer treatment changes from day to day. Fatigue, cognitive effort, and energy for social contact all vary, so an app built around fixed goals and streaks tends to discourage the people it is meant to help. Our team is building a mobile and web health app that supports physical activity, cognitive health, and social connection while adapting to each survivor's capacity on a given day.

## How we are approaching it

- **Co-design with survivors.** Survivors help decide what the app should include, remove, rename, or invent. Features come from their needs rather than our assumptions.
- **Choice over pressure.** The app offers manageable options instead of prescriptions. Rest days count as valid entries, and progress reflects what people actually logged, with no streaks.
- **AI that goes beyond a chatbot.** We are working toward personalized activity recommendations, exercise planning, adaptive content, and plain-language explanations of wearable fitness data.
- **Grounded, private AI.** Recommendations are meant to be grounded in vetted health resources through retrieval and tool calling, while limiting how much sensitive data the model sees.
- **Consent first.** The AI cannot change anything for a user without passing explicit identity, consent, scope, and approval checks.

## What I have built

- The app's frontend in React and TypeScript: home, activities, journal, progress, and profile sections, guided activity sessions, a shared visual system, and a guest mode that works without an account.
- A Django backend with account creation, email verification, login, and password reset, storing signed-in records in PostgreSQL, with tests and an OpenAPI contract.
- The safety layer the AI assistant must pass through before acting: a strict schema for proposed actions, an activity allowlist, and consent and approval gates, all built before any model is connected.
- A one-command Docker setup that builds the full stack, runs migrations, and creates a synthetic demo account.

## Next steps

- Connect the AI assistant and wearable data.
- Evaluate prototypes with survivors through usability tasks, think-aloud sessions, interviews, and questionnaires, and feed what we learn into each design iteration.

## Stack

React · TypeScript · Vite · Tailwind CSS · Django · PostgreSQL · Python · Docker

---

[Profile](https://github.com/adhvikrayaprolu) · [LinkedIn](https://www.linkedin.com/in/adhvikrayaprolu)
