---
layout: post
title: "(Re-updated) Second working post"
date: 2023-10-22 18:43:54
categories: fresh
---
# (updated) Second working post

Ill edit this after the fact

*I have updated this post*

<!-- random quote -->

{% assign quotes = "The only way to do great work is to love what you do.|Don't watch the clock; do what it does. Keep going.|The future depends on what you do today.|Don't watch the clock; do what it does. Keep going.|Success is not the key to happiness. Happiness is the key to success." | split: "|" %}

{% assign random = site.time | date: "%N" | modulo: quotes.size %}

<div class="quote">
  <p>{{ quotes[random] }}</p>
</div>

