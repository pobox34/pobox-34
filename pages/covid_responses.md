---
layout: page
title: Covid Responses
permalink: '/covid-responses/'
---

<div class="exhibit-meta container">
    <h6>The following selections were part of a writing assignment in response to COVID-19 in prisons. During the pandemic, incarcerated people suffered some of the harshest lockdown conditions in history: 2 weeks of full lockdown without access to showers or phone calls, followed by 23.75 hour lockdowns with 15 minutes out to make a phone call or take a shower. During this time, they were not allowed access to outdoor space, and chow halls were shut down to avoid unnecessary movement. Currently, in May 2021, SCI Chester is still operating on a 23 hour lockdown condition, with 1 hour out. Many have been able to go back to work such as at the library, medical ward, barber, multimedia facilities. Needless to say these prolonged isolation periods have taken a severe toll on mental health conditions inside prisons. Furthermore, despite these strict efforts to keep COVID infection rates down, SCI Chester still suffered an outbreak in October 2020, with hundreds of inmates and staff infected. Many are still experiencing lingering effects of the virus, as well as having been in critical condition. Several lives of long-term inmates were lost during this time. This platform was created in effort to provide a space where those incarcerated in the American prison system had a place to write and have their thoughts and voices heard. 
</h6>

    {% assign responses = site.works | where_exp:'work', "work.label contains 'Covid Response'" %}

    {% for response in responses %}
        <div class='row justify-content-md-center'>
            <div class='col-10'>
                <p class="ml-5"><a href="{{site.baseurl}}{{response.permalink}}">{{response.label}}</a></p>
            </div>
        </div>
    {% endfor %}
</div>
