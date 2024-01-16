---
title: Japanese input in openSUSE Tumbleweed
tags: Japanese, input methods, openSUSE
date: 2024-01-15
description: Recently I change from Ubuntu 22.10 to openSUSE Tumbleweed on my personal laptop. Here are the steps to install fcitx5 and fcitx5-mozc input method for Japanese
image: https://images.unsplash.com/photo-1543966888-6e858b90d30d?q=80&w=2023&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA==
draft: false
---

Photo by [Paul Esch-Laurent](https://unsplash.com/@pinjasaur?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash) on [Unsplash](https://unsplash.com/photos/orange-and-pink-computer-keyboard-zZlEcBxJ_Sw?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash)

## Situation

Recently I change from Ubuntu 22.10 to openSUSE Tumbleweed on my personal laptop. The wonderful thing about change is that always brings learning with it.

Here are the steps to install **fcitx5** and **fcitx5-mozc** input method for Japanese in **openSUSE Tumbleweed**:

## Solution

1. Open the terminal and enter the following command to install **fcitx5** and **fcitx5-mozc**[^1]:

   ```shell
   sudo zypper install fcitx5-mozc
   ```

2. Next, if you aren't using a desktop environment [^2] you may need to configure the input method. To do this, create or open a new file called `~/.profile` and add the following lines to it:

   ```shell
   export GTK_IM_MODULE=fcitx
   export QT_IM_MODULE=fcitx
   export XMODIFIERS=@im=fcitx
   ```

3. Save the file and restart your system.

4. Once you have restarted your system, open the **fcitx5 configuration tool** by running the following command in the terminal:

   ```shell
   fcitx5-configtool
   ```

5. In the configuration tool, click on the **Input Method** tab and then click on the **+** button to add a new input method.

6. Select **Mozc** from the list of input methods and click on the **Add** button.

7. You can now switch to the **Mozc** input method by pressing the **Ctrl + Space** keys.

I hope this helps! Let me know if you have any questions.

[^1]: Japanese input in plasma 5.8 kde <https://forums.opensuse.org/t/japanese-input-in-plasma-5-8-kde/125211>
[^2]: Localization/Japanese - ArchWiki. <https://wiki.archlinux.org/title/Localization/Japanese>.
