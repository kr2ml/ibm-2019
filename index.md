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

# Tentative Schedule


| Event                                          | Duration |
|------------------------------------------------|----------|
| (Invited Talk) Title TBD - Andrew McCallum (UMass Amherst)    | 45 mins  |
| L+R Over Graphs: Brandy Freitas (Pitney Bowes) | 30 mins  |
| L+R Over Graphs: Kelsey Allen (MIT)            | 30 mins  |
| Coffee + KR2ML@IBM Posters                     | 30 mins  |
| (Invited Talk) Title TBD - Milind Tambe (Harvard)             | 45 mins  |
| L+R Applications/Systems: Masataro Asai (IBM) | 30 mins  |
| L+R Applications/Systems: Lee Martie (IBM)     | 30 mins  |
| Lunch                                          | 75 mins  |
| (Invited Talk) Title TBD                       | 45 mins  |
| [QA Challenge Session](#qa-challenge-session) + Open Discussion         | 60 mins  |
| Coffee + KR2ML@IBM Posters                     | 30 mins  |
| Open Discussion: *Challenges, Opportunities & Next Steps in Bridging KRR & ML*                                | 90 mins|

Please also check out the rest of the [AI Week](https://ibm.biz/ai-research-week) program.


# QA Challenge<a name="qa-chalenge-session"></a>

This year, we are also organizing a shared task inspired by the challenges encountered when working with real-world enterprise data. End-users interact with AI systems via a natural language interface -- customer support, chatbots, enterprise search, etc. The end-users are not aware of the internal knowledge representation employed by the  AI  system and often lack the expertise to issue structured queries to the underlying knowledge base. 

To this end, we propose a task to automatically translate a natural language query to a structured representation (SPARQL) that can be used to query the underlying knowledge base. 
We will build upon the series of [QALD challenges](http://qald.aksw.org/) and release a set of [training queries](#challenge-train-data) -- natural language queries and their corresponding SPARQL queries. The set of questions will be a subset of previous QALD challenges and will be representative of different real-world issues commonly encountered in such applications (noise, ambiguous language, errors in the knowledge base,  etc.). 

The underlying knowledge base will be DBpedia (2016-10 version), and Wikipedia as the optional text corpus. The participants may use the information present in the structured knowledge base and the unstructured text corpus to understand the natural language query and output the structured representation.  Most of the existing systems for translating natural language queries to structured representation often rely on a set of rules or templates. As a result, such systems are very brittle and fail to perform even with slight variations of the query. To overcome that, generated multiple paraphrasing/variants of the same question to test how sensitive the algorithms are to such changes.

### Examples

Q1:  Give me the currency of China.

Q1a: What is the name of currency used in China?

Q2:  When did Latvia join the EU?

Q2a: When did Latvia become part of the EU?

### Training Data<a name="challenge-train-data"></a>

The training data is available for download now. 

There are 5 tab separated columns in the file:

ID: question id

Original Question : original text of the question

Paraphrasing 1  : paraphrasing of the questions by annotator 1

Paraphrasing 2  : paraphrasing of the questions by annotator 2

SPARQL Query    : SPARQL query for the original question
 
### Test Data

Test Data will be released on 30th August, 2019.

The systems will be evaluated based on the accuracy of retrieved answers via the generated structured representations. Participants should report their train and test accuracies in their presentations/posters during the workshop.



# Workshop Organizers

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
