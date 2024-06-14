---
title: Pages
description: the Pages page for pages
---

This page showcases how to list items in a specific collection.

<ul>
    {% for tool in site.pages %}
        <li>
            <h2>
                <a href="{{ page.url | relative_url }}">
                    {{ page.title }}
                </a>
            </h2>

            <p>
                <i>{{ page.description }}</i>
            </p>
            <p>{{ page.excerpt }}</p>
        </li>
    {% endfor %}
</ul>
