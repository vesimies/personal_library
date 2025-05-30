---
layout: default
title: Resource Library
---

<h1>Resource Library</h1>

<ul>
  {% for resource in site.resources %}
    <li>
      <a href="{{ resource.url }}">{{ resource.title }}</a> - {{ resource.description }}
    </li>
  {% endfor %}
</ul>

<!-- _config.yml -->
title: My Resource Library
baseurl: ""
url: "https://vesimies.github.io"
theme: minima

collections:
  resources:
    output: true
    permalink: /resources/:name/

# Navigation (in _includes/nav.html)
<nav>
  <ul>
    <li><a href="/">Home</a></li>
    <li><a href="/resources/">Resources</a></li>
  </ul>
</nav>

<!-- Sample Resource Markdown (_resources/programming_languages.md) -->
---
title: Programming Languages
description: Useful links for languages I'm learning
layout: resource
---

## Python

- [Python Docs](https://docs.python.org/3/): The official documentation.
- [W3Schools Python](https://www.w3schools.com/python/): Quick syntax guides and examples.

## Git Bash

- [Bash Guide](https://guide.bash.academy/): Simple introduction to Bash scripting.
- [tldr pages](https://tldr.sh/): Short explanations of bash commands with examples.


<!-- Basic CSS (assets/css/style.css) -->
body {
  background-color: #fdfaf5;
  font-family: 'Inter', sans-serif;
  color: #2e2e2e;
  max-width: 700px;
  margin: auto;
  padding: 1rem;
}
a {
  color: #5a7f71;
}
h1 {
  color: #df907a;
}
nav ul {
  list-style: none;
  display: flex;
  gap: 1rem;
  padding: 0;
}
nav li {
  display: inline;
}
