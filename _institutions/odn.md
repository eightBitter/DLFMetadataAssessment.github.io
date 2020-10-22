---
inst_code: odn
name: Ohio Digital Network
---

Led by the State Library of Ohio and in partnership with Ohio Library and Information Network, Ohio Public Library Information Network, and Ohio History Connection, the Ohio Digital Network builds on strong digital collection efforts across the state including Ohio Memory and the Ohio Digitization Hubs project.

<ul>
    {% for spec in site.metadata_specs %}
        {% if spec.institution == "odn" %}
            <li>
                <h2><a href="spec.url">{{ spec.title }}</a></h2>
                <p>{{ spec.content | markdownify }}</p>
            </li>
        {% endif %}
    {% endfor %}
</ul>