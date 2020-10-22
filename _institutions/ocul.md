---
inst_code: ocul
name: OCUL--Scholars Portal
---

Scholars Portal is a service of the Ontario Council of University Libraries (OCUL). Founded in 2002, Scholars Portal provides a shared technology infrastructure and shared collections for all 21 university libraries in the province.

<ul>
    {% for spec in site.metadata_specs %}
        {% if spec.institution == "ocul" %}
            <li>
                <h2><a href="spec.url">{{ spec.title }}</a></h2>
                <p>{{ spec.content | markdownify }}</p>
            </li>
        {% endif %}
    {% endfor %}
</ul>