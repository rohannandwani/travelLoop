https://traveloop-sigma.vercel.app/
# Traveloop

Traveloop is a hackathon-ready travel planning MVP. It turns a natural language trip idea into a multi-city itinerary with editable dates, activities, budgets, discovery search, visual calendars, and share/collaboration controls.

## Run

```bash
npm install
npm run dev
```

Open `http://localhost:3000`.

## MVP Flow

1. Enter a trip idea in the AI prompt.
2. Generate a suggested itinerary across selected cities.
3. Drag activities between calendar days or edit them manually.
4. Track budget by category and city.
5. Share public/friend links and invite collaborators.

The AI and discovery endpoints are deterministic mock services for demo reliability. Swap the generation logic in `app/api/generate-itinerary/route.ts` with an LLM call when API keys are available.

## Deploy For Hackathon Submission

Vercel is the fastest production host for this Next.js MVP.

```bash
npx vercel login
npx vercel --prod
```

Choose the current folder as the project root when prompted. The final `https://...vercel.app` URL is permanent enough for hackathon judging and does not depend on your laptop staying online.
