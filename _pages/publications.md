---
layout: page
permalink: /publications/
title: publications
description: Journal articles grouped by ABDC rank, then book chapters and conference papers, newest first. Use the search box to filter by keyword, co-author, journal or year.
nav: true
nav_order: 2
---

<!-- _pages/publications.md -->

{% include bib_search.liquid %}

<p style="font-size:.9rem">
Full, auto-updated lists: <a href="https://scholar.google.com/citations?user=IOrgqG0AAAAJ&hl=en">Google Scholar</a> ·
<a href="https://orcid.org/0000-0001-7179-3878">ORCID</a> ·
<a href="https://www.scopus.com/authid/detail.uri?authorId=57202530494">Scopus</a>.
Journal ranks follow the ABDC Journal Quality List.
</p>

<p style="font-size:.9rem"><strong>Jump to:</strong>
<a href="#journal-articles-abdc-a">ABDC A</a> ·
<a href="#journal-articles-abdc-b">ABDC B</a> ·
<a href="#journal-articles-abdc-c">ABDC C</a> ·
<a href="#other-refereed-journal-articles">Other journals</a> ·
<a href="#book-chapters">Book chapters</a> ·
<a href="#conference-papers">Conference papers</a></p>

<div class="publications">

<h2 id="journal-articles-abdc-a" style="margin-top:2rem">Journal articles — ABDC A</h2>

{% bibliography --query @*[tier=a] %}

<h2 id="journal-articles-abdc-b" style="margin-top:2rem">Journal articles — ABDC B</h2>

{% bibliography --query @*[tier=b] %}

<h2 id="journal-articles-abdc-c" style="margin-top:2rem">Journal articles — ABDC C</h2>

{% bibliography --query @*[tier=c] %}

<h2 id="other-refereed-journal-articles" style="margin-top:2rem">Other refereed journal articles</h2>

{% bibliography --query @*[tier=other] %}

<h2 id="book-chapters" style="margin-top:2rem">Book chapters</h2>

{% bibliography --query @*[tier=chapter] %}

<h2 id="conference-papers" style="margin-top:2rem">Conference papers</h2>

{% bibliography --query @*[tier=conference] %}

</div>
