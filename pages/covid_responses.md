---
layout: page
title: Covid Responses
permalink: '/covid-responses/'
---

<div class="exhibit-meta container">
    <h6>Here we've published the Writers' responses to the COVID-19 pandemic. Note: due to the sensitive nature of the subject matter, the Writers of these pieces remain Anonymous.</h6>

    {% assign responses = site.works | where_exp:'work', "work.label contains 'Covid Response'" %}

    {% for response in responses %}
        <div class='row justify-content-md-center'>
            <div class='col-10'>
                <p class="ml-5"><a href="{{site.baseurl}}{{response.permalink}}">{{response.label}}</a></p>
            </div>
        </div>
    {% endfor %}
</div>
