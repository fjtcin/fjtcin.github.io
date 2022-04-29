---
layout: page
title: Collaborate With Me
---

# Collaborate With Me
{:.no_toc}

> Hope you'll have a nice trip! :eyes:

## Things to Do
{:.no_toc}

* .
{:toc}

## Install TeX Live

WARNING: 安装时间较长，所需流量较多，请合理选择一段时间进行安装。

1. 在[官网](https://tug.org/texlive/windows.html#install)下载 `install-tl-windows.exe`。

    <p style="text-align:center;"><img src="/assets/collaborate-with-me-latex-1.png" alt="Download Installer"></p>

1. 运行 `install-tl-windows.exe`

    <p style="text-align:center;"><img src="/assets/collaborate-with-me-latex-2.png" alt="Run Installer" width="400"></p>

1. 在弹出的设置窗口中，Uncheck `Install TeXworks front end`，这是因为我们用更美观和强大的 VS Code 做为编辑器。随后点击 `Advanced` 做进一步修改。

    <p style="text-align:center;"><img src="/assets/collaborate-with-me-latex-3.png" alt="Modify Basic Settings" width="400"></p>

1. 在弹出的窗口中，点击图中圈出的 `Customize` 按钮。

    <p style="text-align:center;"><img src="/assets/collaborate-with-me-latex-4.png" alt="Modify Advanced Settings" width="600"></p>

1. Uncheck All languages EXCEPT `Chinese`, `Chinese/Japanese/Korean (base)` and `US and UK English`. This can save you almost 1GB.

    <p style="text-align:center;"><img src="/assets/collaborate-with-me-latex-5.png" alt="Uncheck Unnecessary Languages" width="500"></p>

---

等待完漫长的安装过程后，在命令行输入 `latex -v`，应有类似如下的结果：

<p style="text-align:center;"><img src="/assets/collaborate-with-me-latex-6.png" alt="Installed Successfully" width="700"></p>

否则，请将编译器目录 `XXXX/bin/win32` 添加至 PATH 中。

<p style="text-align:center;"><img src="/assets/collaborate-with-me-latex-7.png" alt="Add PATH" width="500"></p>

## Set Git

根据[知乎上的教程](https://zhuanlan.zhihu.com/p/31417255)一直做到 `3、克隆仓库` 的内容。

注意：在克隆仓库时，应当克隆我们协作用的仓库。

完成后，你就能在本地看到项目的一切文件了。

## Use Git to Collaborate

当你在本地完成某个模块的更新后，输入以下命令，即可完成提交。

```bash
git pull
git add .
git commit -m "SAY SOMETHING ABOUT WHAT YOU HAVE CHANGED"
git push
```

注意，`git add` 后有一个点，不要漏了它。

<p style="text-align:center;"><img src="/assets/collaborate-with-me-git.png" alt="Git CLI"></p>

---

```text
March, 2022; Hefei, China;
Dedicated to my fantastic collaborators.

Please feel free to add a comment if you witness ANY error.
Last modified on 3/8/2022.
```
