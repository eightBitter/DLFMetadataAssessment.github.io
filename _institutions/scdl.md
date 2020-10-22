---
inst_code: scdl
name: South Carolina Digital Library
---

The South Carolina Digital Library provides free access to historic materials illustrating the history and culture of South Carolina from over 40 cultural heritage institutions across the state.

<ul>
    {% for spec in site.metadata_specs %}
        {% if spec.institution == "scdl" %}
            <li>
                <h2><a href="spec.url">{{ spec.title }}</a></h2>
                <p>{{ spec.content | markdownify }}</p>
            </li>
        {% endif %}
    {% endfor %}
</ul>