# CBC Buddy upgraded starter

## What is included
- Responsive phone-first learning interface
- Grade selector for Grades 1–12
- Sample learning cards across nine learning areas
- Mini-lesson prompts, quiz prompts, and fraction example fallback
- AI tutor API endpoint, designed to keep the API key on the server
- Installable PWA shell and basic offline caching

## Run
1. Install Node.js 18 or newer.
2. Run `npm install`.
3. Set `OPENAI_API_KEY` in your hosting environment or terminal.
4. Run `npm start`; open `http://localhost:3000`.

The `.env.example` file is a template only. If you want to use a `.env` file, install `dotenv` and add `import 'dotenv/config';` at the top of `server.js`, or configure environment variables in your hosting dashboard. Never put the API key in browser files.

## Deploy and install on Android
Deploy to a host that supports Node.js and set the secret environment variable in the host settings. Static-only hosting can show the learning interface but needs a serverless/backend function for the AI endpoint. Once deployed over HTTPS, open the website in Android Chrome and choose Install app or Add to Home screen. An APK/AAB requires a separate Android wrapper/build step.

## Important limitations
The uploaded ZIP contained an Android APK/AAB and signing files, not the original editable source. This is therefore a new starter project, not a direct modification of the compiled app. It includes sample learning cards, not all official CBC books or a complete verified Grade 1–12 curriculum. Add only curriculum resources you have permission to use and have teachers review them before claiming full coverage.
