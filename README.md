# Summer Chore Quest 2026

A gamified summer chore tracker for the Roberts family. Three "houses" race to 1,000 points to win the Summer House Cup, with weekly $10 payouts and a reward menu (Pool Day, Movie Night, Fat Cats, and more).

## Pages

- **index.html** — landing page with links to both views
- **chore_dashboard.html** — read-only family scoreboard
- **chore_control_center.html** — parent-only control panel (phone-optimized)

## How to run

Open `index.html` in any modern browser. Works offline. State is saved in your browser's localStorage.

## Hosting on GitHub Pages

1. Create a new repository (e.g., `chore-quest`)
2. Upload these three HTML files to the root
3. Settings → Pages → Source: `main` branch / root → Save
4. Wait 30 seconds, then visit `https://<your-username>.github.io/chore-quest/`

## How the rotation works

Each kid is assigned one of three chore sets, rotating weekly:

| Cycle slot | Adaline | Avery | Rhett |
|------------|---------|-------|-------|
| 1          | Set A   | Set B | Set C |
| 2          | Set B   | Set C | Set A |
| 3          | Set C   | Set A | Set B |

Two bonus chores (vacuum downstairs, big trash cans) rotate separately. Mon–Sat are chore days; Sunday is review/payout day.

## Scoring

- Each chore is worth points (3–15 each). Max ~243 pts/week per kid.
- Earn 80% of your weekly points → automatic $10 payout.
- Remaining points fill your "points bank" — spend on rewards or save for the House Cup.
- Every point earned counts toward your House total. First house to 1,000 wins the Summer House Cup.

## Note on cross-device sync

Data is stored in each device's browser. For shared access, either:
- Use one shared device as the source of truth
- Use the Export/Import JSON buttons in Settings to back up and move data
- Host with a real backend (Firebase/Supabase) for live sync — TBD

