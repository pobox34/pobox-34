---
layout: page
title: About
permalink: /about/
---



This website aims to connect incarcerated writers with a wider audience, including writing mentors and educators, collaborators from the international visual arts community, musicians, performers, people who express creatively. I hope this will open up conversation and ultimately get feedback, correspondence & connection to the writers and artists in prison.

The world is burning.

We have set up a [GoFundMe](http://gf.me/u/yp8fys) page to raise funds to keep the project running. Thank you for your support!

Please send writing submissions, artwork, & inquiries to PO Box 34, Collingswood, NJ. 08108, USA or email pobox34@protonmail.com.

## PO Box 34 would like to thank the following organizations for their Support:
<div class='album'>
    <div class='container'>
        <div class='row'>
            {% for logo in site.about.logos %}
                <div class='col-md-4'>
                    <a href='{{ logo.link }}' title='{{ logo.label }}'>
                        <img src='{{ logo.img | absolute_url }}'>
                    </a>
                </div>
            {% endfor %}
        </div>
    </div>
</div>
