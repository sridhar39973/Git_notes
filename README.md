# Git and Bitbucket: Guide and Hands-on Labs

A small, offline-friendly website for getting confident with Git, versioning and Bitbucket in a team setting. It has a reference guide and a lab workbook with 10 hands-on labs and a progress tracker.

No build step, no dependencies, no JavaScript framework. Plain HTML and CSS, plus a few lines of JavaScript for the lab progress bar.

## What is inside

| File | Purpose |
|---|---|
| `index.html` | The guide: 15 short chapters (how Git works, SSH, cloning, branching, merging, conflicts, pull requests, rebase, undoing mistakes, tags and versioning, deleting repos, extras, cheat sheet, practice lab) |
| `labs.html` | The workbook: 10 hands-on labs, 46 tick-box steps, a "you should see" check and a fix for common mistakes in each lab |
| `style.css` | Shared styles for both pages (light and dark mode follow your system) |
| `labs.css` | Extra styles for the workbook |

Keep all four files in the same folder.

## How to use it

1. Open `index.html` in a browser (double-click the file). Read a chapter, then try the commands.
2. Click **Start the hands-on labs** (or open `labs.html`) and work through the labs in order.
3. Tick each step as you finish it. Your progress is saved in your browser (local storage), so it stays on that device and browser only.
4. Create a free Bitbucket Cloud account first. Every lab uses a throwaway practice repository.

In the commands, replace `WORKSPACE` with your own Bitbucket workspace ID (the part of the URL right after you sign in).

## The 10 labs

1. Account and SSH
2. First repo: create, clone, commit and push
3. Branches: create, publish and delete
4. A full pull request: comment, update, merge and clean up
5. A merge conflict with a "teammate" (two clones of one repo)
6. A conflict inside a pull request
7. The undo toolkit: restore, amend, revert, stash and reflog
8. Versioning: semantic versions, tags and `npm version`
9. Bitbucket Pipelines: tests that run on every push, including a deliberate failure
10. Deploy stages (staging, then manual production) and a capstone that simulates a day on the job

## Getting to "confident"

- Do one or two labs a day.
- Repeat labs 5 and 6 until they feel boring.
- Finish the capstone (lab 10, part B) without notes, then tick the confidence checklist at the end of the workbook.

That is a reasonable test that you are ready for a team repository. It does not replace practice on real work.

## Good to know

- **Windows:** run the commands in Git Bash (installed with Git for Windows), so `echo`, `cat` and `>>` behave as shown.
- **Free plan limits:** Bitbucket Pipelines gives a limited number of build minutes per month. Check the current allowance in your workspace billing page before re-running builds often.
- **Pull requests on a one-person account:** you may not be able to approve your own pull request. Merge it yourself if the Merge button is available.
- **Deployment lab:** the staging and production steps only print a message. They teach the structure and how to promote a release, not a real server deploy. A real deploy replaces the `echo` with an upload or deploy command, and credentials belong in secured repository variables, never in the code or the YAML file. Ask your team which deploy target they use (for example AWS) and learn that command in your first week.
- **Bitbucket changes:** menu names and plan limits change over time. If a screen looks different, follow what you see and check Bitbucket's documentation.
- **Safety:** use practice repositories only. Do not delete or force-push anything that belongs to a real project.

## Not covered

Git hooks, submodules, advanced history rewriting, and any cloud-specific deployment. These can be added as extra chapters or labs.

## Hosting it (optional)

To get a link you can open on any device, push the folder to a GitHub repository and turn on GitHub Pages (Settings, then Pages, then deploy from the `main` branch). The site works the same when hosted.
