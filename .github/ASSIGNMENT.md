# 📄 Ocarina of Time Guide

Build a four-page fan guide to The Legend of Zelda: Ocarina of Time, and practice linking
pages together into a real website.

## 🎯 Overview

Last time, you built a single web page. Real websites have many pages that share the same
header, navigation, and footer, and link to each other. In this exercise, you will build
**Ocarina of Time Guide**, a small fan site for the Nintendo Switch 2 remake of
**Ocarina of Time**, with four pages:

- **Home**, which introduces the game and links to the rest of the guide
- **Controls**, which lists every button and how to save
- **Ocarina Songs**, which shows four songs as button sequences on a text music staff
- **Deku Tree Walkthrough**, a step-by-step guide to the first dungeon, kept in its own folder

Each page focuses on a different group of HTML elements. Together, they teach you how to
build a site that people can move around in.

There is no CSS in this exercise, so the pages will look plain when you are finished.
**That is expected.** Right now, the focus is on structure and links. Later, CSS will let you
control colors, fonts, layout, and spacing.

## 🧠 What You Will Learn

By completing this exercise, you will practice how to:

- Build a shared `header`, `nav`, and `footer`, and repeat them on every page
- Link pages together with relative paths, including into and out of a folder (`../`)
- Link to other websites, open them in a new tab, and create an email link
- Jump to a section of a page with `id` and `#` links
- Organize content with `section`, `article`, `aside`, and `div`, and know when to use each
- Show text exactly as typed with `pre`, and show buttons and keys with `kbd`
- Group an image or other content with its caption using `figure` and `figcaption`
- Add contact information with `address`
- Leave notes in your code with HTML comments
- Show special characters such as ©, &, and ← with character entities

## 📂 Starter Files

| File | What you will practice |
| --- | --- |
| `index.html` | Page structure: `section`, `article` cards inside a `div`, and an image in a `figure` |
| `controls.html` | `kbd` for buttons, an ordered list of steps, and an `aside` that links to another page |
| `songs.html` | Four songs as text music staffs in `pre`, each inside a `figure` with a `figcaption` |
| `walkthrough/deku-tree.html` | Links with `../`, jump links with `id`, a nested list, an `aside`, and an image one folder up |
| `images/` | The two images used on Home and on the Deku Tree page |

Every page starts with two lines that are **not** visible page content:

```
Page title: Controls: Ocarina of Time Guide
Page description: Every default button in the Ocarina of Time remake ...
```

They belong in the `head`. Use the first as the page's `title` and the second as the
`content` of a `<meta name="description">` element, then delete the labels.

## 📋 Requirements

### Every page

- [ ] Has a `DOCTYPE`, `html` (with `lang="en"`), `head`, and `body`
- [ ] The `head` has `<meta charset="utf-8">`, a viewport `meta`, the page's own `title`, and
      its own `meta` description from the starter text
- [ ] Has the same `header`, `nav`, `main`, and `footer` as every other page
- [ ] The site name in the `header` links to the Home page
- [ ] The `nav` links are a `ul`, with each link in its own `li`
- [ ] Has exactly one `h1`, and the rest of the headings follow the page's outline
- [ ] Has HTML comments that label the header, main content, and footer

### Links

- [ ] Every page's `nav` links to all four pages with **relative** paths
- [ ] On `walkthrough/deku-tree.html`, every link to another page uses `../`
      (for example, `../index.html`)
- [ ] The footer links to Nintendo's Zelda website and Zelda Wiki with **absolute** URLs, and
      both open in a new tab with `target="_blank"`
- [ ] The email address in the footer is a `mailto:` link
- [ ] The "Jump to" links on the Deku Tree page go to sections with matching `id`s
- [ ] The `aside` on the Controls page links to the *Hum It Instead* section of the Songs page
      (`songs.html#humming`)

### Page structure

- [ ] On Home, *About the Remake* and *What's in This Guide* are each a `section`
- [ ] On Home, each of the three guide cards is an `article`, and the three `article`s are
      wrapped in one `div`
- [ ] The *Rather Hum Than Press Buttons?* box on Controls and the *Pro Tip* on the Deku Tree
      page are each an `aside`
- [ ] The Deku Tree route is an `ol`, with the smaller steps nested as an `ol` inside each
      main step's `li`
- [ ] The save steps on Controls are an `ol`

### Buttons and songs

- [ ] Every button name on Controls is marked up with `kbd` (for example,
      `<kbd>ZL</kbd>`)
- [ ] Each of the four song staffs on the Songs page is inside a `pre`, and the columns still
      line up in the browser
- [ ] Each staff and its *Play:* line are wrapped in a `figure`, with the *Play:* line as the
      `figcaption`
- [ ] Every button in each *Play:* line is its own `kbd`

### Images

- [ ] The image placeholder on Home is replaced with an `img` that points to
      `images/link-and-navi.jpg`
- [ ] The image placeholder on the Deku Tree page is replaced with an `img` that points to
      `../images/queen-gohma.jpg`
- [ ] Each image and its caption are wrapped in a `figure`, with the caption in a `figcaption`
- [ ] Each image has `alt` text that describes what it shows
- [ ] Both images display on the live site

### Contact info and special characters

- [ ] The contact lines in the footer are inside an `address`, with a `br` at the end of each
      line except the last
- [ ] The © in every footer is written as `&copy;`
- [ ] Every & in the page text is written as `&amp;`
- [ ] The ← on the Deku Tree page is written as `&larr;`

## 🧮 Grading

| Criteria | What earns full credit | Points |
| --- | --- | --- |
| **Every page** | Correct document structure on all four pages; each page has its own `title` and `meta` description; the same `header`, `nav`, `main`, and `footer` on every page; one `h1` per page. | 2 |
| **Links** | All `nav` links work on every page, including `../` links from the walkthrough folder; absolute links open in a new tab; the `mailto:` link works; jump links and the cross-page link land on the right sections. | 4 |
| **Page structure** | `section`, `article`, `div`, and `aside` are used where the requirements call for them; the nested route list and the save steps are `ol`s. | 2 |
| **Buttons and songs** | Buttons use `kbd`; each song staff is a `pre` inside a `figure` with a `figcaption`, and the staffs line up in the browser. | 2 |
| **Images** | Both images display on the live site from the correct paths, inside `figure`s with `figcaption`s, with descriptive `alt` text. | 2 |
| **Comments, contact info, and characters** | HTML comments label the main parts of each page; the footer contact info is in an `address` with `br`s; ©, &, and ← use character entities. | 2 |
| **Published and submitted** | GitHub Pages site is live and loads correctly; pull request into `main` is open with the live URL in the description; PR URL submitted in Canvas. | 1 |
| **Total** |  | **15** |

## ✅ Before You Submit

Check the following:

- [ ] Every page has your markup, and none of the "Page title:" or "Page description:" labels
      appear on any page
- [ ] No `[replace this ...]` lines are left on Home or the Deku Tree page
- [ ] You did not rename or move any of the starter files
- [ ] On the **live site**, you clicked every `nav` link on every page, including from the
      Deku Tree page, and each one opened the right page
- [ ] The "Jump to" links and the link to *Hum It Instead* land on the right sections
- [ ] Both images show up, on a computer and on your phone
- [ ] The song staffs line up in the browser
- [ ] Each browser tab shows that page's own title
- [ ] Every page passes the [W3C Markup Validator](https://validator.w3.org/#validate_by_input)
      with no errors
- [ ] You saved all of your files
- [ ] The site is live on GitHub Pages and the URL is in your pull request

## 🛠️ Troubleshooting

If something is not working, check these common issues first:

- **A link goes to a "404" or "file not found" page?** Check the file name and folder in the
  `href`, letter for letter. From the Deku Tree page, every link to another page needs `../`.
- **The Deku Tree image is broken, but the Home image works?** The Deku Tree page is one folder
  down, so its `src` needs `../images/` instead of `images/`.
- **The song staffs are squished onto one line?** The staff needs to be inside a `pre`. Without
  it, the browser removes the extra spaces and line breaks.
- **A jump link doesn't move the page?** The `href` after the `#` must match the `id` exactly,
  including dashes.
- **The email link opens nothing?** That's normal in some browsers and in WebStorm's built-in
  preview if no email app is set up. Check that the `href` starts with `mailto:`.
- **The © shows up as strange characters?** Add `<meta charset="utf-8">` to the `head`, and use
  `&copy;`.
- Did you save every file? Are your opening and closing tags in the correct places, and nested
  properly? Are there quotation marks around your attribute values?

## 📚 Resources

- [MDN — HTML elements reference](https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements)
- [MDN — Creating links](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Structuring_content/Creating_links)
- [MDN — Document and website structure](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Structuring_content/Structuring_documents)
- [MDN — `figure`](https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/figure)
- [MDN — Entity (special characters)](https://developer.mozilla.org/en-US/docs/Glossary/Entity)
- [W3C Markup Validation Service](https://validator.w3.org/#validate_by_input): paste your
  HTML in to catch unclosed tags

---

The AI policy and submission instructions are in the [README](../README.md).
