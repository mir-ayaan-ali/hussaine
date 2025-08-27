---
layout: default
title: Search
permalink: /search/
---
<h1 style="font-family:Georgia,serif;">Search</h1>
<input id="search-input" class="search-input" placeholder="Type to search posts…" autofocus />
<ul id="results-container" class="search-results"></ul>

<script src="https://unpkg.com/simple-jekyll-search@latest/dest/simple-jekyll-search.min.js"></script>
<script>
  SimpleJekyllSearch({
    searchInput: document.getElementById('search-input'),
    resultsContainer: document.getElementById('results-container'),
    json: '{{ '/search.json' | relative_url }}',
    searchResultTemplate: '<li><a href="{url}">{title}</a> <span class="badge">{date}</span></li>',
    noResultsText: 'No results',
    fuzzy: true,
    limit: 20
  });
</script>
