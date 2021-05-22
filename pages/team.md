---
layout: page
title: Team
permalink: /team/
---
<div class='team'>
    {% for item in site.data.team %}
        <h3>{{ item.title }}</h3>
        {% if item.people %}
            {% for person in item.people %}
                {% if item.title == "Project Team" %}
                    <div class='container'>
                        <div class='row justify-content-md-center'>
                            <div class='col-5'>
                                <h4><a href=
                                "{{ site.baseurl }}/writers/{{ person.link }}">
                                    {{ person.name }}
                                </a></h4>
                            </div>
                        </div>
                    </div>
                {% else %}
                <div class='media'>
                    <img src='{{ person.img | absolute_url }}' height='200'>
                    <div class='media-body'>
                        <h4>{{ person.name }}</h4>
                        <p>{{ person.bio }}</p>
                    </div>
                </div>
                {% endif %}
            {% endfor %}
        {% endif %}
    {% endfor %}
</div>

