# claude-new-features-guide

Companion repo for the video **"7 New Ways to Use Claude in 10 Minutes (Meetings, Boards, Sheets and More)"** by David Oluyale | Agentic AI Hub.

It has every copy-paste prompt, command and pause-and-try exercise from the video. One example runs through the whole thing: planning a small public workshop called **"Build with Claude"**.

> Features and plan availability change often. What you see depends on your plan and account. The notes below say exactly what the recording account showed.

## Video chapters

| Time | Chapter |
|---|---|
| 0:00 | Intro: 7 new Claude features |
| 0:26 | 1. Meetings (Team and Enterprise) |
| 1:36 | 2. Whiteboards |
| 3:25 | 3. Sheets |
| 4:33 | 4. Data |
| 5:42 | 5. Interactive Connectors |
| 6:39 | 6. Themes (Claude Desktop) |
| 7:54 | 7. Advisor (Claude Code) |
| 9:12 | Quick quiz and recap |

## The 7 features

### 1. Meetings
**What it is:** Claude joins a Google Meet call as its own participant. It takes notes, answers questions in the chat, and can start a doc or a board. After the call, the notes, action items and anything it made are on one meeting page.

**Plan:** it's a beta for Team and Enterprise plans only. The account in the video doesn't have a Meetings item, so the video shows no live call.

**Pause and try:** on a Team or Enterprise plan, open **Meetings** in the sidebar, look at one upcoming call and find **Add Claude**. Don't add it unless you mean to. If you don't see a Meetings item, your plan doesn't have it yet.

### 2. Whiteboards
**What it is:** a shared board inside Claude. Turn a messy plan into a timeline, a list and a checklist. To change one part, drag a box around it and ask Claude to edit only that area.

**Pause and try:** paste the [whiteboard prompt](PROMPTS.md#whiteboard). Then box one area and paste the [edit prompt](PROMPTS.md#whiteboard-edit-one-area).

Note: before it edited, Claude asked two quick questions. In the video I clicked Skip, so it used placeholder roles and dates.

### 3. Sheets
**What it is:** a spreadsheet Claude builds with you, with tabs, formulas and drop-downs, all from one prompt.

**Pause and try:** build the tracker with the [Sheets prompt](PROMPTS.md#sheets). Then change one estimated cost and use the [follow-up prompt](PROMPTS.md#sheets-follow-up).

The Budget formula in the video (cell D2) was `=IF(B2="","",B2-C2)`. If the estimated cost is blank, the cell stays blank.

### 4. Data
**What it is:** dashboards and data stories built from a connected data source, such as a warehouse or a CRM. It used to be called Claude Dashboards.

**What the recording account showed:** no Data item in the sidebar and no data source connected, so there's no dashboard in the video and no numbers were made up.

**Pause and try:** if you have a data connector, use the [Data prompt](PROMPTS.md#data) for one real dashboard. If you don't, just open your connector list and note a source you might add.

### 5. Interactive Connectors
**What it is:** some connectors can open as a live app beside your chat, or full screen. It's rolling out on the web and in the Claude desktop app.

**What the recording account showed:** no Interactive badge on its connectors, so the video tours the connectors directory and connects no new account.

**Pause and try:** open the connectors directory and see what's listed. Don't connect a new tool unless you mean to. If you already have an interactive one, try the [Connectors prompt](PROMPTS.md#interactive-connectors).

### 6. Themes (Claude Desktop, with Claude Code)
**What it is:** in the Claude desktop app, `/theme` sets the appearance (`system`, `light` or `dark`). For an animated backdrop behind the chat, install Anthropic's official **Theme Examples** plugin and pick a scene with `/custom-theme`. You can apply a scene to a project or to just one session.

```text
/theme
/plugin install theme-examples@claude-plugins-official
/custom-theme
/custom-theme Halftone Dusk session
```

**Pause and try:** type `/custom-theme`, preview one scene, then apply it to this session only.

### 7. Advisor (Claude Code)
**What it is:** your main model can ask a stronger model for help at key moments, for example before it commits to a plan or when it's stuck. Type `/advisor` to turn it on and pick the advisor model. Claude decides when to use it. It's experimental and can use more tokens, so keep an eye on `/usage`.

```text
/advisor
```

**Pause and try:** turn on `/advisor`, then plan one function with the [Advisor prompt](PROMPTS.md#advisor). Read the plan before you accept any code.

In the video, Claude returned a plan with 6 steps, 8 edge cases, and the first test it would write (rejecting a duplicate sign-up). The screen didn't show a separate advisor step, so the video doesn't claim one.

## Quick quiz

1. **Which plans can use Claude Meetings today, and which video app does it join?** Team and Enterprise plans, in beta. Right now it joins Google Meet.
2. **On a whiteboard, how do you ask Claude to change only one part?** Drag a box around that part, then ask Claude to edit only that area.
3. **In Claude Code, what does `/advisor` do?** It lets your main model consult a stronger model at key decisions, like before it commits to a plan or when it's stuck.

## Files

- [`PROMPTS.md`](PROMPTS.md): every copy-paste prompt from the video.
