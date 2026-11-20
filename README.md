# 💻 Ocarina of Time Guide

Starter files for a multi-page HTML coding exercise. You will build a four-page fan guide to
**The Legend of Zelda: Ocarina of Time**, remade for Nintendo Switch 2 in 2026. Along the way,
you will link pages together, organize a site into folders, and publish it with GitHub Pages.

The pages are going to look plain in the browser, and that is fine. There is no CSS in this
exercise. The point is to practice using HTML to organize a whole site, not just one page.
Styling comes later in the course.

> [!NOTE]
> `.editorconfig`, `.gitattributes`, `.gitignore`, `.noai`, and the `.github` and `.idea`
> folders are setup files that keep assignments consistent. Leave them alone. The four `.html`
> files and the `images` folder are your starter files.

## 📋 Assignment Requirements

> [!IMPORTANT]
> **Start here: [read ASSIGNMENT.md →](.github/ASSIGNMENT.md)**

It has the overview, the requirements, the grading criteria, and a final checklist. Read it before you start, and check it again before you submit.

## ✅ At a Glance

Every assignment follows the same steps. Each guide has screenshots for every step.

| Step | What you do                                                                | Guide                                         |
|------|----------------------------------------------------------------------------|-----------------------------------------------|
| 0    | **First assignment only:** install and set up WebStorm                     | [WebStorm Setup](.github/WEBSTORM_SETUP.md)   |
| 1    | Create your repo from this template, clone it, and make a `develop` branch | [Getting Started](.github/GETTING_STARTED.md) |
| 2    | Mark up the starter pages where they are                                   | [Where Your Files Go](#-where-your-files-go)  |
| 3    | Commit and push often, then turn on GitHub Pages                           | [Publishing](.github/PUBLISHING.md)           |
| 4    | Open a pull request into `main` and submit its URL in Canvas               | [Submitting](.github/SUBMITTING.md)           |

## 📂 Where Your Files Go

This time the files are already named and in the right places. Each `.html` file holds plain
text with no HTML in it yet. Open each one and add your markup around the text that is
already there. **Do not rename or move the files**, because the links between pages depend
on these exact names and folders.

When you are finished, your repo should look like this:

```
index.html
controls.html
songs.html
images/
    link-and-navi.webp
    queen-gohma.webp
walkthrough/
    deku-tree.html
```

`index.html` stays in the root folder, the same folder as this README. GitHub Pages publishes
from the root, so your site will 404 without it.

> [!TIP]
> `walkthrough/deku-tree.html` lives one folder down. Its links and images have to go back
> **up** a folder with `../` to reach the other pages and the `images` folder. The videos walk
> you through it.

## 🤖 AI Policy

Work on this assignment must be your own. Do not use AI coding assistants — including
GitHub Copilot, Cursor, ChatGPT, Claude, or JetBrains AI Assistant — to generate,
complete, or rewrite your code.

You should be able to explain any line of your submission. You may be asked to do so.

This repo includes a `.noai` file, which disables JetBrains AI Assistant for the project
in IDEs like WebStorm. Leave it in place. It is a reminder of the policy above, not a
substitute for it — following the policy is still your responsibility.

> [!NOTE]
> The `.noai` file does **not** turn off WebStorm's local Full Line code completion. Turn that
> off yourself as part of the [one-time setup](.github/WEBSTORM_SETUP.md) (step 5).

> [!CAUTION]
> Late or missing submissions are graded on what is in the pull request at the deadline, so push your final commits
> before you submit.
