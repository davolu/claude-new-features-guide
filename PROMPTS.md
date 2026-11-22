# Prompts from the video

Paste these into a new Claude chat. They match the pause-and-try moments in the video.

## Whiteboard

```text
Start a whiteboard to plan a small public workshop called 'Build with Claude'. Include a simple timeline, a session list, and a checklist for the week before the event.
```

## Whiteboard: edit one area

First drag a box around the timeline on the board, then send:

```text
Add owners and dates to only the boxed timeline. Keep the rest of the board the same.
```

## Sheets

```text
Create a sheet to track the 'Build with Claude' workshop. Add a Tasks tab with columns for task, owner, status as a dropdown, and due date. Add a Budget tab with item, estimated cost, actual cost, and a formula for the remaining amount.
```

## Sheets follow-up

Change one estimated cost on the Budget tab, then send:

```text
I changed one estimated cost. Please update the remaining total on the Budget tab.
```

## Data

Only if a data source is already connected. Real figures only.

```text
Make a simple one-page dashboard for one metric I already have in this connected source. Show only real figures from the connector, and say when the data was last refreshed.
```

## Interactive Connectors

Only if you already have an interactive connector set up.

```text
Open my already connected interactive tool beside this chat. Do not connect a new account.
```

## Advisor

In Claude Code, run `/advisor` first, then send:

```text
Plan one small function that records a workshop sign-up: name, email, and session choice. Do not write the code yet. List the steps, the edge cases, and one test you would add first.
```

## Desktop commands (Themes and Advisor)

```text
/theme
/plugin install theme-examples@claude-plugins-official
/custom-theme
/custom-theme Halftone Dusk session
/advisor
```
