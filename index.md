---
layout: page
title: KR2ML
subtitle: Knowledge Representation & Reasoning Meets Machine Learning
use-site-title: true
---
## Date: 9/19/19, 9 am to 6 pm
## Location: Coming Soon (Cambridge MA)

# About

Machine learning (ML) has seen a tremendous amount of recent success, and has been applied in a variety of applications. However, some of these methods come with several drawbacks, such as the need for large amounts of training data, and the lack of explainability and verifiability of the results. In many domains, there is structured knowledge (e.g., from electronic health records, laws, clinical guidelines, or common sense knowledge) which can be leveraged for reasoning in an informed way (i.e., including the information encoded in the knowledge representation itself) in order to obtain high quality answers. Symbolic approaches for knowledge representation and reasoning (KR) are less prominent today - mainly due to their lack of scalability - but their strength lies in the verifiable and interpretable reasoning that can be accomplished. This workshop aims at the intersection of these two sub-fields of AI, and hopes to shine a light on the synergies that exist between KR and ML.

# Tentative Schedule: 


| Event                                          | Duration |
|------------------------------------------------|----------|
| (Invited Talk) Title TBD - Andrew McCallum (UMass Amherst)    | 45 mins  |
| L+R Over Graphs: Brandy Freitas (Pitney Bowes) | 30 mins  |
| L+R Over Grpahs: Kelsey Allen (MIT)            | 30 mins  |
| Coffee + KR2ML@IBM Posters                     | 30 mins  |
| (Invited Talk) Title TBD - Milind Tambe (Harvard)             | 45 mins  |
| L+R Applications/Systems: Achille Fokoue (IBM) | 30 mins  |
| L+R Applications/Systems: Lee Martie (IBM)     | 30 mins  |
| Lunch                                          | 75 mins  |
| (Invited Talk) Title TBD                       | 45 mins  |
| QA Challenge Session + Open Discussion         | 60 mins  |
| Coffee + KR2ML@IBM Posters                     | 30 mins  |
| Open Discussion: *Challenges, Opportunities & Next Steps in Bridging KRR & ML*                                | 90 mins|

Please also check out the rest of the [AI Week](https://ibm.biz/ai-research-week) program.


# Organizers

- [Veronika Thost](https://researcher.watson.ibm.com/researcher/view.php?person=ibm-Veronika.Thost)
- [Kartik Talamadupula](http://www.ktalamad.com/)
- [Sumit Bhatia](http://sumitbhatia.net/)
- Hima Karanam

<!-- <div class="posts-list">
  {% for post in paginator.posts %}
  <article class="post-preview">
    <a href="{{ post.url | prepend: site.baseurl }}">
	  <h2 class="post-title">{{ post.title }}</h2>

	  {% if post.subtitle %}
	  <h3 class="post-subtitle">
	    {{ post.subtitle }}
	  </h3>
	  {% endif %}
    </a>

    <p class="post-meta">
      Posted on {{ post.date | date: "%B %-d, %Y" }}
    </p>

    <div class="post-entry-container">
      {% if post.image %}
      <div class="post-image">
        <a href="{{ post.url | prepend: site.baseurl }}">
          <img src="{{ post.image }}">
        </a>
      </div>
      {% endif %}
      <div class="post-entry">
        {{ post.excerpt | strip_html | xml_escape | truncatewords: site.excerpt_length }}
        {% assign excerpt_word_count = post.excerpt | number_of_words %}
        {% if post.content != post.excerpt or excerpt_word_count > site.excerpt_length %}
          <a href="{{ post.url | prepend: site.baseurl }}" class="post-read-more">[Read&nbsp;More]</a>
        {% endif %}
      </div>
    </div>

    {% if post.tags.size > 0 %}
    <div class="blog-tags">
      Tags:
      {% if site.link-tags %}
      {% for tag in post.tags %}
      <a href="{{ site.baseurl }}/tags#{{- tag -}}">{{- tag -}}</a>
      {% endfor %}
      {% else %}
        {{ post.tags | join: ", " }}
      {% endif %}
    </div>
    {% endif %}

   </article>
  {% endfor %}
</div>

{% if paginator.total_pages > 1 %}
<ul class="pager main-pager">
  {% if paginator.previous_page %}
  <li class="previous">
    <a href="{{ paginator.previous_page_path | prepend: site.baseurl | replace: '//', '/' }}">&larr; Newer Posts</a>
  </li>
  {% endif %}
  {% if paginator.next_page %}
  <li class="next">
    <a href="{{ paginator.next_page_path | prepend: site.baseurl | replace: '//', '/' }}">Older Posts &rarr;</a>
  </li>
  {% endif %}
</ul>
{% endif %} -->
