# TeamClock (demo)

A small demo of a staff sign-in and hours tracker for small businesses. It uses made-up sample people and rates. It is a test sample, not a finished product, and not payroll.

## What it does

**Staff view**
- Clock in and out with one button
- See this week's hours split into normal and overtime
- See a rough estimate of gross pay (normal, overtime, total) and the month so far
- See next week's scheduled hours and approved days off
- Request time off and see whether it was approved

**Manager view**
- See who is clocked in right now
- See the whole team's hours and estimated gross pay for the week
- Approve or decline time-off requests
- Export the week as a CSV file to use in another system
- AI helper: paste a message such as "Dave forgot to clock out, he left at 5" and get a suggested correction to approve. A second button reviews the week and flags anything unusual.

## Important notes

- Pay figures are rough gross estimates only, before tax, National Insurance, holiday pay and pension. This is not payroll.
- Overtime is anything over a person's contracted weekly hours, at 1.5 times their rate. These rules are simple assumptions for the demo.
- The AI helper does not do any pay sums. Plain code calculates hours and pay. The AI only reads messages, flags problems and explains them.
- The AI buttons only work in the Claude-hosted version of the demo. In a plain copy of this page they are switched off, and everything else still works.
- Demo data is saved in your browser only. There are no logins and no server.

## Run it

Open `index.html` in a browser. Or serve the folder:

```
python3 -m http.server 8000
```

To host it free, turn on GitHub Pages for this repository (Settings, Pages, deploy from the main branch).

## Built with

Plain HTML, CSS and JavaScript in a single file. Built with AI assistance (Claude).

## What I would build next

- Real logins and a database so each person uses their own phone
- A weekly rota with scheduled vs actual hours
- Shift swap requests
- A server route for the AI helper, with the API key kept on the server and rate limiting
- Links to other systems beyond CSV export

## Licence

MIT. See `LICENSE`.
