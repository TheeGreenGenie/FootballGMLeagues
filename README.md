# Football GM Leagues

This repository contains Football GM league data and two summary reports:

- `yearly_report.txt` — season-by-season player and team rankings
- `career_report.txt` — career and all-time rankings across players, draft classes, rookies, and teams
- `base_leagues/` — league JSON files for each season
- `draftclasses/` — draft class JSON files used to build draft rankings

================================================================================

## Downloading and Opening the Files

1. Clone or download the repository

   - If this project is hosted on GitHub or another Git provider, clone it with:
     ```powershell
     git clone <repo-url>
     cd footballGMLegaues
     ```

   - If you downloaded a ZIP archive, extract it and open the extracted folder.

2. Open the reports

   - Use a plain text editor to open `yearly_report.txt` and `career_report.txt`.
   - On Windows, you can also view them in PowerShell:
     ```powershell
     Get-Content .\yearly_report.txt | more
     Get-Content .\career_report.txt | more
     ```

3. Use the supporting data files

   - `base_leagues/` contains season JSON data for the leagues.
   - `draftclasses/` contains draft JSON files used to generate rookie and draft-class summaries.
   - These JSON files are the underlying data sources for the reports.

## What `yearly_report.txt` Offers

`yearly_report.txt` covers season-level rankings and team performance across the covered years.

Sections included in this file:

- `Y1. TOP 10 TEAMS PER SEASON (avg OVR of top-22 rostered players)`
  - Lists the best team by roster strength for every season.
  - Includes each team’s average overall and the top 3 players for context.

- `Y2. BEST UNIT CHAMPION PER YEAR (group #1 team every season)`
  - Identifies the strongest unit or team group each season.
  - Helpful for seeing which team had the best overall roster performance.

- `Y3. TOP 15 PER POSITION — EVERY SEASON`
  - Ranks the best players at each position for every season.
  - Useful for position-specific scouting insights.

- `Y4. POSITION AVERAGE OVR BY SEASON (trend table)`
  - Tracks how average player overall ratings change over time by position.
  - Great for identifying era trends and positional peaks.

- `Y5. BEST POSITIONAL UNITS PER TEAM — EVERY SEASON (detailed)`
  - Highlights the top positional combinations for each team in every season.
  - Shows which teams had standout units on offense, defense, or special groups.

================================================================================

## What `career_report.txt` Offers

`career_report.txt` summarizes career-level and all-time rankings from players, draft classes, rookies, and team-seasons.

Sections included in this file:

- `C1. TOP 200 SINGLE-SEASON OVERALLS`
  - Ranks the absolute best single-season player ratings.
  - Includes the player, position, season, team, and overall score.

- `C2. TOP 100 CAREER AVERAGE OVERALLS`
  - Lists the best career average ratings across eligible players.
  - Includes years played, season span, average overall, and peak overall.

- `C3. CAREER AVERAGE OVR — ASCII CHARTS BY POSITION (top 50 per pos)`
  - Provides graphical trend charts for position-level career averages.
  - Helps compare career trajectory across different positions.

- `C4. PLAYER DEVELOPMENT`
  - Tracks player development patterns and peaks over career timelines.
  - Useful for scouting improvement and longevity analysis.

- `C5. BEST PLAYERS IN EACH DRAFT CLASS (top 5 per class)`
  - Identifies the elite rookies from each year’s draft.
  - Shows which draft years delivered the strongest top picks.

- `C6. DRAFT CLASSES RANKED BY STRENGTH (avg of top-25 OVR)`
  - Ranks draft classes by the average strength of their top players.
  - Useful for evaluating draft depth and class quality.

- `C7. BEST ROOKIES (top 75 by rookie-season OVR)`
  - Ranks the best rookie seasons across all draft classes.
  - Highlights immediate impact newcomers.

- `C8. ALL-TIME TOP 50 PER POSITION (best single season)`
  - Lists the best single seasons for each position across history.
  - Useful for all-time comparisons and positional legends.

- `C9. ALL-TIME BEST TEAM-SEASON UNITS — TOP 50 PER GROUP`
  - Ranks the strongest team-season units in the dataset.
  - Shows the best combined performance of teams and units.

================================================================================

## Tips for Working with the Reports

- Use the long `=` header blocks as reliable section delimiters when searching or parsing the files.
- Search for `Y1.`, `Y2.`, `C1.`, `C2.`, etc. to jump directly to the category you need.
- The files are designed for readability and for use as a data summary layer on top of the JSON league source files.

Enjoy exploring the Football GM yearly and career rankings data.
