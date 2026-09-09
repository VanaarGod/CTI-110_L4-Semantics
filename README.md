# CTI-110 L4 — Semantic HTML Page

Welcome to your fourth web development assignment! In this exercise, you'll create a new GitHub repository, clone it into VS Code, and build a webpage using **semantic HTML tags** instead of generic `<div>` containers.

## Step 1: Create Your Repository

1. Go to [GitHub](https://github.com) and log in.
2. Click **New repository**.
3. Name your repository exactly:
   ```
   CTI-110_L4-Semantics
   ```
4. Set the repository to **Public**
5. Check the box to **Add a README file**.
6. Click **Create repository**.

## Step 2: Clone Your Repository into VS Code

1. Open VS Code.
2. Click Clone Git Repository
3. Select your repository in the dropdown at the top of your screen.
4. Save it within a "GitHub" folder on your computer.
5. When prompted, click **Open** to open the cloned repository folder in VS Code.

> ‼️If you haven't already, navigate to your Extensions Store in VS Code and install "Live Server." You'll know you've found the right one if it has over 81,000,000 downloads!

## Step 3: Create Your HTML File

1. In the VS Code file explorer (left sidebar), create a new file named:
   ```
   index.html
   ```
2. On the very first line of your file, type `!` and then press the **Tab** key to generate the HTML boilerplate.
3. Update the `<title>` tag inside the `<head>` section with your **First and Last name**.

## Step 4: Choose Your Topic

Pick a topic of your choice for your page — examples include a favorite hobby, a sport, a place you'd like to visit, a movie or show, or a piece of technology.

> ‼️Your topic just needs to give you enough content to fill out the sections below. Run it by me if you're unsure it will work.

## Step 5: Build Your Page with Semantic HTML — No `<div>` Tags Allowed

This assignment is about **semantic structure**. Instead of wrapping content in generic `<div>` tags, you'll use HTML tags that describe what the content actually *is*. Build out your `<body>` using the following elements:

- **`<header>`** — Tells the browser "this is the introductory content for the page." Include a page heading (`<h1>`) with your topic's title.
- **`<nav>`** — Tells the browser "this is a block of navigation links." Include a short list of links representing a simple navigation menu for your page. See below for how to build this with placeholder links.
- **`<main>`** — Tells the browser "this is the primary content of the page," as opposed to sidebars, navigation, or repeated header/footer content. Wrap your primary page content in a `<main>` tag. A page should only have **one** `<main>` element.
  - **`<section>`** — Groups a chunk of related content under a general theme, usually with its own heading. Use at least **two** `<section>` elements to divide your page into distinct topic areas (e.g., "Overview" and "Details").
  - **`<article>`** — Marks content that could stand completely on its own, independent of the rest of the page (like a blog post, a news story, or a review someone could copy/paste elsewhere and it would still make sense). Inside one of your sections, include at least **one** `<article>` element containing a self-contained piece of content (e.g., a fact, a review, or a short story related to your topic).
  - **`<aside>`** — Marks content that's related to the nearby content but not essential to it — the "by the way" of a page (like a sidebar tip, a fun fact, or a related link). Include an `<aside>` element with related but secondary content.
- **`<footer>`** — Tells the browser "this is the closing content for the page," typically things like credits, copyright, or contact info. Include a footer with a closing line, such as your name and the current year.

> ‼️If you catch yourself typing `<div>`, stop and ask which semantic tag actually describes that content instead.

### Building Your `<nav>` with Placeholder Links

Your navigation menu doesn't need real destinations yet — you're just practicing the structure. Wrap your links in an unordered list inside the `<nav>` tag, and use `#` as the `href` value to create a placeholder (or "dead") link that doesn't go anywhere when clicked:

```html
<nav>
  <ul>
    <li><a href="#">Home</a></li>
    <li><a href="#">Overview</a></li>
    <li><a href="#">Details</a></li>
  </ul>
</nav>
```

Each `<a href="#">` is a real, clickable link — it just points to the top of the current page instead of a different page. This lets you build out the navigation structure now and wire up real page links later.

## Step 6: Add Images

Add at least **2 images** to your page using `<img>` tags.

- Use the `src` attribute to link to an image (either a local file in your repository or a URL).
- Every image **must** include an `alt` attribute describing the image.

## Step 7: Add Your Lists

Somewhere within your sections or article, include:

- At least **one** ordered list (`<ol>`) with `<li>` items.
- At least **one** unordered list (`<ul>`) with `<li>` items.

## Step 8: Use Semantic Text Tags

Instead of using non-semantic formatting shortcuts, use the following tags within your content:

- **`<strong>`** — for text that needs strong importance (instead of just bolding it visually).
- **`<em>`** — for text that needs emphasis (instead of just italicizing it visually).
- **`<br>`** — for a line break where one is actually needed within a block of text.

> ‼️No CSS yet! This assignment is only about structure and semantics — styling comes in a later assignment.

## Step 9: Test Your Page

Test your site using the **Live Server** extension:

1. Right-click your `index.html` file in the VS Code file explorer.
2. Select **"Open with Live Server."**
3. Your page will open in a browser tab so you can check your work.

## Step 10: Submit Your Work with Git

Once your page looks correct, submit it using Git:

1. Open a new **Terminal** in VS Code.
2. Run the following commands one at a time:

```bash
git add .
git commit -m "COMMIT MESSAGE GOES HERE"
git push
```

> ‼️Replace `"COMMIT MESSAGE GOES HERE"` with a short, descriptive message about what you did (e.g. `"Completed Semantics assignment"`).

## Step 11: Publish Your Site with GitHub Pages

Once your work is pushed to GitHub, turn your repository into a live website:

1. On GitHub, go to your `CTI-110_L4-Semantics` repository page.
2. Click the **Settings** tab.
3. In the left sidebar, click **Pages**.
4. Under **Build and deployment**, set the **Source** to **Deploy from a branch**.
5. Under **Branch**, select **main** (or **master**) and keep the folder set to **/ (root)**.
6. Click **Save**.
7. Wait a minute or two, then refresh the Pages settings screen. GitHub will display a link like:
   ```
   https://your-username.github.io/CTI-110_L4-Semantics/
   ```
8. Click the link to view your live site.

> ‼️Every time you `git push` new changes, GitHub Pages will automatically update your live site within a minute or two.

> ‼️GitHub Pages defaults to render your README.md file unless it finds an "index.html" file in the root folder. Always make sure your home page is set to "index.html"! This is case sensitive.

---

### Checklist Before You Submit
- [ ] Repository `CTI-110_L4-Semantics` created on GitHub
- [ ] Repository cloned into VS Code
- [ ] `index.html` file created inside the cloned repo
- [ ] HTML boilerplate generated with `!` + `Tab`
- [ ] `<title>` updated with your First and Last name
- [ ] Page includes a `<header>` with an `<h1>`
- [ ] Page includes a `<nav>` with a list of links
- [ ] Page content is wrapped in `<main>`
- [ ] At least 2 `<section>` elements used
- [ ] At least 1 `<article>` element used
- [ ] At least 1 `<aside>` element used
- [ ] Page includes a `<footer>`
- [ ] **No `<div>` tags anywhere in the page**
- [ ] At least 2 images included, each with an `alt` attribute
- [ ] At least 1 ordered list (`<ol>`) included
- [ ] At least 1 unordered list (`<ul>`) included
- [ ] `<strong>`, `<em>`, and `<br>` tags each used at least once
- [ ] No CSS used
- [ ] Page tested with Live Server
- [ ] Work committed and pushed with Git commands in the VS Code Terminal
- [ ] GitHub Pages enabled in repository Settings
- [ ] Live site link verified and working
- [ ] ‼️YOU MUST SUBMIT CLICKABLE LINKS TO YOUR GITHUB REPOSITORY AND YOUR LIVE SITE THROUGH GITHUB PAGES. 2 LINKS. BOTH CLICKABLE OR YOU WILL RECEIVE A ZERO.