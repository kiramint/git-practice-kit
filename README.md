# git-practice-kit

**中文：** 本仓库仅作为 [git-practice-lab](https://github.com/kiramint/git-practice-lab) 的 **submodule 练习目标**。请勿 fork 本仓库当作主作业；主练习请 fork `git-practice-lab`。

**English:** This repository exists **only** as a git submodule target for the Git practice lab. Do **not** fork this repo for the main homework — fork `kiramint/git-practice-lab` instead.

## Files

| Path | Purpose |
|------|---------|
| `kit/VERSION` | Version string learners can inspect after adding the submodule |
| `kit/TIPS.md` | Short tips about cloning and updating submodules |

## For learners

In Stage 4 of the lab assignment you will run something like:

```bash
git submodule add https://github.com/kiramint/git-practice-kit.git third_party/kit
```

Then explore `third_party/kit/` and commit the submodule pointer in the parent repo.
