# Commands Used

## 1. Fork & Clone
`git clone <url>` — downloads the repo's full history to my local machine and sets up `origin` pointing to my fork.

## 2. Add name file & commit
`git add Vinayak.txt` — stages the file for commit.
`git commit -m "2026-09-06"` — snapshots the staged file with the date as the message.

## 3. Create branch
`git branch Vinayak` — creates a new pointer at the current commit; doesn't switch to it.

## 4. Switch & add roll number file
`git checkout Vinayak` — moves HEAD to point at the Vinayak branch.
`git add RollNumber.md` / `git commit -m "Add self-description"` — stages and commits the new file.

## 5. Add commit hash
`git log -1 --format="%H"` — prints the full hash of the latest commit.
Appended the hash into RollNumber.md, then committed again.

## 6. Merge
`git checkout main` — switch back to main.
`git merge Vinayak` — fast-forwards main's pointer to include Vinayak's commits (since main hadn't moved).

## 7. Edit README
Appended my name, staged, committed.

## 8. Add dish & reset
Appended dish, staged, committed — then:
`git reset --hard HEAD~1` — moved main's pointer back one commit and discarded the dish line entirely from the working directory.

## 9. commands.md
This file itself, documenting everything above.

## 10. Push & PR
`git push origin main` — pushes local main branch to my fork on GitHub.
Then opened a pull request via GitHub's UI.
