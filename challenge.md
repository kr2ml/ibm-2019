---
layout: page
title: KR2ML
subtitle: Knowledge Representation & Reasoning Meets Machine Learning
use-site-title: true
---
## Date: 9/19/19, 9 am to 5 pm
## Location: MIT, Cambridge MA (Room TBD)
## Go to [Registration](https://kr2ml.eventbrite.com)

<hr>

# QA Challenge<a name="qa-chalenge-session"></a>

This year at KR2ML, we are organizing a shared task inspired by the challenges encountered when working with real-world enterprise data. End-users interact with AI systems via a natural language interface -- customer support, chatbots, enterprise search, etc. The end-users are not aware of the internal knowledge representation employed by the  AI  system and often lack the expertise to issue structured queries to the underlying knowledge base. 

To this end, we propose a task to automatically translate a natural language query to a structured representation (SPARQL) that can be used to query the underlying knowledge base. 
We will build upon the series of [QALD challenges](http://qald.aksw.org/) and release a set of [training queries](#challenge-train-data) -- natural language queries and their corresponding SPARQL queries. The set of questions will be a subset of previous QALD challenges and will be representative of different real-world issues commonly encountered in such applications (noise, ambiguous language, errors in the knowledge base,  etc.). 

The underlying knowledge base will be DBpedia (2016-10 version), and Wikipedia as the optional text corpus. The participants may use the information present in the structured knowledge base and the unstructured text corpus to understand the natural language query and output the structured representation.  Most of the existing systems for translating natural language queries to structured representation often rely on a set of rules or templates. As a result, such systems are very brittle and fail to perform satisfactorily when faced with even slight variations of the query. To overcome that, multiple paraphrasing/variants of the same question were generated to test how sensitive the algorithms are to such changes.


### Examples


`Q1:  Give me the currency of China.` <br />
`Q1a: What is the name of currency used in China?`

`Q2:  When did Latvia join the EU?` <br />
`Q2a: When did Latvia become part of the EU?`

### Training Data<a name="challenge-train-data"></a>

The training data is [available for download now](https://kr2ml.github.io/ibm-2019/qa-challenge/kr2ml_train.tsv). 

There are 5 tab separated columns in the file:

`ID`: question id <br />
`Original Question`: original text of the question <br />
`Paraphrasing 1` : paraphrasing of the questions by annotator 1 <br />
`Paraphrasing 2` : paraphrasing of the questions by annotator 2 <br />
`SPARQL Query`: SPARQL query for the original question <br />
 
### Test Data & Evaluation<a name="challenge-test-data"></a>

<!-- Test Data will be released on 30th August, 2019. -->

The test data is [available for download now](https://kr2ml.github.io/ibm-2019/qa-challenge/challenge_test.tsv).

The test file is a tab separated file with the following columns:

`ID`: question id <br />
`Question`: a natural language question <br />

You will be required to produce the SPARQL query that can be used to answer the question from DBpedia corpus specified above.

You are required to submit the output produced by your system in a single tab separated file with three columns:

`ID`: question id <br />
`Question`: a natural language question <br />
`Output SPARQL`: SPARQL query as produced by your system <br />

Note that each line corresponds to one natural language question. Please make sure that there are no line-breaks in the SPARQL query.

The systems will be evaluated based on the accuracy of retrieved answers via the generated structured representations. Participants should report their train and test accuracies in their presentations/posters during the workshop.

#### Technical Report

You are also required to submit a brief description of your approach in the form of a technical report/arXiv paper. The paper should provide sufficient details for the readers to understand and replicate your approach. 

### Deadline

The deadline for submission of results is 10th September, 2019.

The results will be announced during the challenge session in the workshop.

### Contact

Please email your submissions, and direct any questions to [sumitbhatia@in.ibm.com](mailto:sumitbhatia@in.ibm.com).





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
