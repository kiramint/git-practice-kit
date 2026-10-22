# Submodule 小贴士 / Tips

1. **带 submodule 的仓库要完整 clone**：使用 `git clone --recurse-submodules <url>`；若已经 clone 过，再执行 `git submodule update --init --recursive`。
2. **父仓库只记录指针**：子模块目录里是另一个独立仓库；父仓库提交的是子模块当前 commit 的 SHA，不是子模块里的全部文件内容。
3. **更新子模块指针**：进入子模块目录拉取新提交后，回到父仓库会看到 `third_party/kit` 有改动，需要再 `add` + `commit` 一次，把新的 SHA 记进父仓库。
4. **Detached HEAD 很常见**：进入子模块后经常处于 detached HEAD。若要在子模块里改代码，先在子模块里建分支、提交并 push，再回父仓库更新指针。
5. **Clone 完子目录是空的？**：多半忘记初始化 submodule。执行 `git submodule update --init`（或带 `--recursive`）即可。
