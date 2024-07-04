# Week 3: Jake Learns to Code

## Table of Contents

- [How to Clone a Repo](#how-to-clone-a-repo)
- [What is Semantic HTML?](#what-is-semantic-html)
- [Navbar Structure](#navbar-structure)
- [Adding an External Stylesheet](#adding-an-external-stylesheet)
- [Styling the Navbar](#styling-the-navbar)
- [Adding Pages](#adding-pages)
- [Adding Content](#adding-content)
- [Resources](#resources)

### How to Clone a Repo

To clone a repository, first visit the relevant GitHub URL, in this case: [https://github.com/BrenLong/teach-jake-week-3](https://github.com/BrenLong/teach-jake-week-3)

1. Click the "Code" dropdown, copy the URL
2. Create a new folder on your computer and drag it into VS Code
3. Open the Terminal in VS Code by clicking `View > Terminal`
4. In the Terminal, type `git clone` and paste in the URL that you copied previously
5. We now have our own local copy of the repo that we can work on and view in our browser
6. Click the "Go Live" extension in VS Code.
7. Now we can make any changes we want and they will be reflected in the browser

### What is Semantic HTML?

Semantic HTML refers to HTML that introduces meaning to the web page rather than just presentation. For example, `<article>`, `<footer>`, and `<header>` are all considered semantic because they accurately describe the purpose of the element and the type of content that is inside them.

#### Why is it important?

Semantic HTML clearly defines the content's structure, making websites more accessible and understandable to both users and search engines. It enhances SEO, ensures compatibility across various devices, simplifies maintenance, and promotes cleaner code.

### Navbar Structure

Here is the structure of our header and navbar using semantic HTML.

Add this directly under the `<body>` tag in index.html

```html
<header>
  <nav class="menu">
    <ul>
      <li>
        <a href="index.html">Home</a>
      </li>
      <li>
        <a href="week1.html">Week 1</a>
      </li>
      <li>
        <a href="week2.html">Week 2</a>
      </li>
      <li>
        <a href="week3.html">Week 3</a>
      </li>
    </ul>
  </nav>
</header>
```

### Adding an External Stylesheet

1. Create an "assets" folder in the root directory.
2. Create a new file in the "assets" folder called `styles.css`.
3. To add the external stylesheet, link it within the `<head>` section of your HTML document: `<link rel="stylesheet" href="assets/styles.css">`.
4. Ensure the "href" attribute points to the correct path where your CSS file is located.

### Styling the Navbar

Here's the code we're using to style our navbar:

```css
body {
  background-color: rgb(205, 123, 123);
}

.menu {
  display: flex;
  justify-content: space-between;
  padding: 1rem 2rem;
  background: #cfd8dc;
}

.menu ul {
  display: flex;
  list-style: none;
}

.menu li {
  padding-left: 1rem;
}

.menu a {
  text-decoration: none;
  color: #0d47a1;
}

.menu a:hover {
  color: #e91e63;
}
```

During the session, we also spoke about nested CSS, click [here](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_nesting/Using_CSS_nesting) to learn more about it.

### Adding Pages

To add a new page to our website, create a new HTML file in the root directory.

For example, to create a "Week 3" page, create a new file called `week3.html`.

### Adding Content

To add content to your new pages, use the same structure as the index.html file.

For example, to add the nav bar to the "Week 3" page, copy the whole `<header>` section from index.html and paste it just below the opening `<body>` tag in `week3.html`.

### Resources

- Cloning a repo: [GitHub Docs](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository)
- Semantic HTML: [MDN Web Docs](https://developer.mozilla.org/en-US/docs/Glossary/Semantics)
- Semantic navbar: [MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/nav)
- Three ways to add CSS: [W3Schools](https://www.w3schools.com/css/css_howto.asp)
- Nested CSS: [MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_nesting/Using_CSS_nesting)
