---
layout: page
title: college
permalink: /college/
---

<ul class="post-list">
    {% for post in site.college%}
        <li>
        <!--Set background image thumbnail-->
        <div class="college-thumbnail" style='background: url("{{post.img}}");'>
        <a href="{{ post.url | prepend: site.baseurl }}"><span class="college-descr">
            <h1>{{ post.title }}</h1>
            <br/>
            <p>{{ post.description }}</p>
        </span></a>
        </div>             
        </li>
    {%endfor%}
</ul>