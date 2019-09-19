---
layout: page
title: KR2ML
subtitle: Knowledge Representation & Reasoning Meets Machine Learning
use-site-title: true
---
## Date: 9/19/19, 9 am to 5 pm
## Location: [MIT Samberg Conference Center](https://whereis.mit.edu/?go=E52)
## Room: *Salon M*
## Go to [Registration](https://kr2ml.eventbrite.com)

<hr>

# About

Machine learning (ML) has seen a tremendous amount of recent success, and has been applied in a variety of applications. However, some of these methods come with several drawbacks, such as the need for large amounts of training data, and the lack of explainability and verifiability of the results. In many domains, there is structured knowledge (e.g., from electronic health records, laws, clinical guidelines, or common sense knowledge) which can be leveraged for reasoning in an informed way (i.e., including the information encoded in the knowledge representation itself) in order to obtain high quality answers. Symbolic approaches for knowledge representation and reasoning (KRR) are less prominent today - mainly due to their lack of scalability - but their strength lies in the verifiable and interpretable reasoning that can be accomplished. This workshop aims at the intersection of these two sub-fields of AI, and hopes to shine a light on the synergies that exist between KRR and ML.

# Tentative Schedule

<span style="color:red">Please visit the [detailed schedule](schedule.md) for full details of all the talks and sessions.</span>


| Event                                          | Time |
|------------------------------------------------|----------|
| Workshop Welcome  |   |
| (Keynote) [Andrew McCallum](https://people.cs.umass.edu/~mccallum/) (UMass Amherst)    | 09:00 - 09:45  |
| L+R Graph Representations                                | 09:45 - 10:30  |
| - [Kelsey Allen](https://cbmm.mit.edu/about/people/allen) (MIT)                           |          |
| - [Ferran Alet](http://web.mit.edu/alet/www/) (MIT)                             |          |
| - [Lee Martie](https://researcher.watson.ibm.com/researcher/view.php?person=ibm-Lee.Martie) (IBM) | |
| Coffee + [KR2ML@IBM Posters](#poster-session)                     | 10:30 - 11:00  |
| (Keynote) [Milind Tambe](https://www.seas.harvard.edu/directory/mtambe) (Harvard)             | 11:00 - 11:45  |
| L+R New Combinations                       | 11:45 - 12:30 |
| - [Masataro Asai](https://researcher.watson.ibm.com/researcher/view.php?person=ibm-Masataro.Asai) (IBM)                       |           |
| - [Achille Fokoue](https://researcher.watson.ibm.com/researcher/view.php?person=us-achille) (IBM) | | 
| - [Lucian Popa](https://researcher.watson.ibm.com/researcher/view.php?person=us-lpopa) (IBM) | | 
| Lunch                                          | 12:30 - 14:00  |
| (Keynote) [Tim Finin](https://www.csee.umbc.edu/~finin/) (UMBC)                     | 14:00 - 14:45  |
| L+R Over Graphs | 14:45 - 15:45 |
| - [Alfio Gliozzo](https://researcher.watson.ibm.com/researcher/view.php?person=us-gliozzo) (IBM)  |   |
| - [Ganesh Ramakrishnan](https://www.cse.iitb.ac.in/~ganesh/) (IIT Bombay) |  |
| - [Lingfei Wu](https://researcher.watson.ibm.com/researcher/view.php?person=us-wuli) (IBM)                                          |          |
| Coffee + [KR2ML@IBM Posters](#poster-session)                     | 15:45 - 16:15  |
| [QA Challenge Session](challenge.md)        | 16:15 - 17:00  |
| - [Sumit Bhatia](https://researcher.watson.ibm.com/researcher/view.php?person=in-sumitbhatia) (IBM) | |
| - Challenge Participants  | |
| - [Tengfei Ma](https://researcher.watson.ibm.com/researcher/view.php?person=ibm-Tengfei.Ma1) (IBM) | |
| Workshop Closing  |   |

Please also check out the rest of the [AI Week](https://ibm.biz/ai-research-week) program.

# QA Challenge 

Please [click here](challenge.md) for full details of the KR2ML 2019 QA Challenge session.



# Poster Session<a name="poster-session"></a>

We invite all IBMers working on combinations of symbolic knowledge representation/reasoning and machine learning to send us posters to display at the workshop. The poster session is intended to act as a showcase of KR2ML work within IBM to the community at large. The idea of our poster session is to give an insight into the wide variety of work in this particular area done at IBM. The poster session is non-archival, and we welcome work that has been presented at other venues previously, etc. Please send your posters, as well as any questions, to [Veronika.Thost@ibm.com](mailto:veronika.thost@ibm.com).

You can find a [list of accepted posters here](schedule.md#poster-session).



# Workshop Organizers<a name="organizers"></a>

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
