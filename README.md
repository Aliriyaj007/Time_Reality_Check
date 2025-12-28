# ⏱️ Time Reality Check

**A brutally honest tool that reveals the gap between how long you think tasks take and how long they actually take.**

---

## Why This Exists

Humans are terrible at estimating time. This isn't opinion — it's documented psychology.

We consistently believe tasks will take less time than they actually do. This leads to:

* Broken schedules
* Missed deadlines
* Chronic stress
* Unrealistic commitments

**What people usually do:**

| Approach                             | Result                          |
| ------------------------------------ | ------------------------------- |
| Guess and hope                       | Consistently wrong              |
| Add "buffer time" arbitrarily        | Still wrong, just differently   |
| Use complex project management tools | Overkill for personal awareness |
| Ignore the problem                   | Repeat the cycle forever        |

**Why existing solutions fail:**

Most productivity tools assume your estimates are correct. They help you *schedule* tasks, not *understand* your estimation bias. They optimize output without addressing the root cause.

> "This tool exists because self-awareness requires measurement, not motivation."

---

## What It Does

* Captures your time estimate before you start a task
* Runs a simple timer while you work
* Compares estimate vs. actual when you finish
* Tracks your bias pattern over time
* Visualizes whether you under/overestimate consistently
* Stores everything locally — nothing leaves your device

**What it does NOT try to be:**

* A project management system
* A team collaboration tool
* A productivity gamification app
* A calendar or scheduler

---

## Before / After

| Before                              | After                               |
| ----------------------------------- | ----------------------------------- |
| "I think this will take 30 minutes" | "I thought 30 min, it took 52 min"  |
| No record of estimation patterns    | Visual trend of your bias over time |
| Repeat the same mistakes            | Calibrate through repeated feedback |
| Guilt and confusion                 | Data and clarity                    |

---

## Sample Output

### Task Completion View

```
┌─────────────────────────────────────┐
│  Task: Write project documentation  │
├─────────────────────────────────────┤
│  Estimated:  30 min   ████████░░░░  │
│  Actual:     52 min   █████████████ │
├─────────────────────────────────────┤
│  Result: Underestimated by 73%      │
└─────────────────────────────────────┘
```

### Statistics Dashboard

```
┌──────────────────┬──────────────────┐
│  Total Tasks: 24 │  Avg Bias: +41%  │
├──────────────────┼──────────────────┤
│  Underestimated: │  Overestimated:  │
│        18        │        4         │
└──────────────────┴──────────────────┘
```

### History Entry

```
Task                  Est    Actual   Bias
─────────────────────────────────────────────
Write documentation   30m    52m      +73%
Fix login bug         15m    23m      +53%
Review PR             10m    8m       -20%
Database migration    60m    94m      +57%
```

---

## Installation & Usage

### Option 1: Direct Browser (Recommended)

No installation required. Download and open.

```bash
# Download the HTML file
curl -O https://raw.githubusercontent.com/Aliriyaj007/Time_Reality_Check/main/index.html

# Open in browser
open index.html        # macOS
xdg-open index.html    # Linux
start index.html       # Windows
```

### Option 2: Git Clone

```bash
git clone https://github.com/Aliriyaj007/Time_Reality_Check.git
cd Time_Reality_Check
open index.html
```

### Option 3: Direct Download

1. Download the latest release: **Download ZIP**
2. Extract the archive
3. Open `index.html` in any modern browser

### Option 4: Serve Locally (Development)

```bash
# Using Python
python -m http.server 8000

# Using Node.js
npx serve .

# Using PHP
php -S localhost:8000
```

Then open `http://localhost:8000` in your browser.

---

## One-Command Usage

```bash
curl -sO https://raw.githubusercontent.com/Aliriyaj007/Time_Reality_Check/main/index.html && open index.html
```

**That's it.** No build step. No dependencies. No configuration.

---

## Configuration

### Themes

Seven built-in themes, switchable via Settings panel:

| Theme         | Description                       |
| ------------- | --------------------------------- |
| Light         | Clean default for daytime use     |
| Dark          | Reduced eye strain for night work |
| Ocean         | Calming blue tones                |
| Forest        | Nature-inspired greens            |
| Sunset        | Warm orange palette               |
| Purple        | Deep violet aesthetic             |
| High Contrast | Accessibility-focused             |

Theme preference persists in `localStorage`.

### Data Storage

All data stored in browser `localStorage` under key: `timeRealityCheck`

```javascript
{
  "tasks": [
    {
      "id": 1234567890,
      "name": "Task name",
      "estimate": 30,
      "actual": 52,
      "completedAt": "2025-01-15T10:30:00.000Z"
    }
  ],
  "theme": "dark"
}
```

### Export Formats

| Format | Use Case                             |
| ------ | ------------------------------------ |
| JSON   | Full backup, re-import capable       |
| CSV    | Spreadsheet analysis, external tools |

---

## Use Cases

**Students**

* Track study session estimates vs. reality
* Identify which subjects take longer than expected
* Plan exam prep more realistically

**Developers**

* Log implementation time against estimates
* Build personal velocity data
* Improve sprint planning accuracy

**Freelancers**

* Understand true project duration
* Quote clients more accurately
* Reduce scope creep surprises

**Remote Workers**

* Audit daily task planning
* Identify time sinks
* Communicate realistic timelines

**Anyone Planning Their Day**

* Stop over-committing
* Build buffer time based on data
* Reduce end-of-day guilt

---

## Limitations

| Limitation               | Reason                                    |
| ------------------------ | ----------------------------------------- |
| Browser-only storage     | Privacy-first design; no sync             |
| No mobile app            | Single HTML file; works in mobile browser |
| No team features         | Individual self-awareness tool            |
| No calendar integration  | Intentionally minimal scope               |
| Clears with browser data | Export regularly if data matters          |

---

## Contributing

Contributions welcome. Keep it simple.

1. Fork the repository
2. Create a feature branch
3. Make changes to `index.html`
4. Test across modern browsers
5. Submit a pull request with clear description

---

## License

MIT License © 2025 Riyajul Ali

---

## Author

**Riyajul Ali**

* GitHub: [https://github.com/Aliriyaj007](https://github.com/Aliriyaj007)
* Email: [aliriyaj007@protonmail.com](mailto:aliriyaj007@protonmail.com)
* LinkedIn: [https://linkedin.com/in/Aliriyaj007](https://linkedin.com/in/Aliriyaj007)

> Built to remove friction, not add features.
