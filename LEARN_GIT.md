# Learn Git — Step by Step 🪜

Hi Zoe! 👋 This guide will walk you through the basics of Git.
Just follow each step in order. Take your time — you can't break anything!

Open the **Terminal** app on your computer and type each command, then press **Enter**.

---

## Step 1 — Get the project onto your computer (clone)

"Cloning" means downloading a copy of the project from GitHub.

```bash
git clone https://github.com/rjclo/zoe_learn_git.git
```

Then move into the project folder:

```bash
cd zoe_learn_git
```

💡 *Tip:* `cd` means "change directory" (go into a folder).

---

## Step 2 — See which branch you are on

A "branch" is like a separate workspace where you can make changes safely.

```bash
git branch
```

You will see a list of branches. The one with a `*` next to it is the one you are currently on (probably `main`).

---

## Step 3 — Create your own branch

Let's make a branch just for you. Replace `zoe-changes` with any name you like
(no spaces — use dashes instead).

```bash
git checkout -b zoe-changes
```

💡 *What this does:* `-b` creates a **new** branch and switches to it at the same time.

Check it worked:

```bash
git branch
```

Now the `*` should be next to `zoe-changes`. 🎉

---

## Step 4 — Make a change

Now for the fun part! Do **one** of these:

**Option A — Edit an existing file**
Open `recipes/pancakes.md` in a text editor and change something
(for example, add "2 bananas" to the ingredients). Save the file.

**Option B — Add a brand-new file**
Create a new file in the `notes/` folder, for example `notes/my-first-note.md`,
and write anything you like inside it. Save the file.

---

## Step 5 — See what you changed

```bash
git status
```

Git will show your changed or new files in red. This just means Git has noticed them
but hasn't saved them yet.

---

## Step 6 — Stage your change (add)

"Staging" tells Git which changes you want to save.

```bash
git add .
```

💡 *Tip:* The `.` means "all my changes". Run `git status` again — your files
should now be green. ✅

---

## Step 7 — Save your change (commit)

A "commit" is a saved snapshot with a short message describing what you did.

```bash
git commit -m "My first change"
```

You can put any message you like inside the quotes.

---

## Step 8 — Send it to GitHub (push)

"Pushing" uploads your branch and commit to GitHub.

```bash
git push -u origin zoe-changes
```

(Use the same branch name you picked in Step 3.)

---

## Step 9 — See it online! 🌐

Go to the repo on GitHub:

👉 https://github.com/rjclo/zoe_learn_git/branches

You should see your branch `zoe-changes` listed. Click on it to view your change.
You did it! 🎉💛

---

## Cheat Sheet 📋

| What you want to do | Command |
| --- | --- |
| Download the project | `git clone <url>` |
| See your branches | `git branch` |
| Make & switch to a new branch | `git checkout -b <name>` |
| Switch to an existing branch | `git checkout <name>` |
| See what changed | `git status` |
| Stage all changes | `git add .` |
| Save a snapshot | `git commit -m "message"` |
| Upload to GitHub | `git push` |

---

### If you ever get stuck

- `git status` is your best friend — run it anytime to see where you are.
- Don't worry about mistakes; branches keep the main project safe.
- Ask Richard for help anytime 💛
