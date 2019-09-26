---
layout: page
title: KR2ML
subtitle: Knowledge Representation & Reasoning Meets Machine Learning
use-site-title: true
---
## Date: 9/19/19, 9 am to 5 pm
## Location: [MIT Samberg Conference Center](https://whereis.mit.edu/?go=E52)
## Room: *Salon M* (7th Floor)
## Go to [Registration](https://kr2ml.eventbrite.com)

<hr>

# Workshop Report

The [workshop report](/docs/kr2ml2019-report.pdf) is now available for download!

# Detailed Schedule


| Event                                          | Time |
|------------------------------------------------|----------|
| Workshop Welcome  |   |
| (Keynote) [Andrew McCallum](#andrew-mccallum) (UMass Amherst)    | 09:00 - 09:45  |
| L+R Graph Representations                                | 09:45 - 10:30  |
| - [Kelsey Allen](#kelsey-allen) (MIT)                           |          |
| - [Ferran Alet](#ferran-alet) (MIT)                             |          |
| - [Lee Martie](#lee-martie) (IBM) | |
| Coffee + [KR2ML@IBM Posters](#poster-session)                     | 10:30 - 11:00  |
| (Keynote) [Milind Tambe](#milind-tambe) (Harvard)             | 11:00 - 11:45  |
| L+R New Combinations                       | 11:45 - 12:30 |
| - [Masataro Asai](#masataro-asai) (IBM)                       |           |
| - [Achille Fokoue](#achille-fokoue) (IBM) | |
| - [Lucian Popa](#lucian-popa) (IBM) | | 
| Lunch                                          | 12:30 - 14:00  |
| (Keynote) [Tim Finin](#tim-finin) (UMBC)                     | 14:00 - 14:45  |
| L+R Over Knowledge Graphs | 14:45 - 15:30 |
| - [Alfio Gliozzo](#alfio-gliozzo) (IBM)  |   |
| - [Ganesh Ramakrishnan](#ganesh-ramakrishnan) (IIT Bombay) | | 
| - [Lingfei Wu](#lingfei-wu) (IBM)                                          |          |
| Coffee + [KR2ML@IBM Posters](#poster-session)                     | 15:30 - 16:15  |
| [QA Challenge Session](challenge.md)        | 16:15 - 17:00  |
| - Sumit Bhatia (IBM) | |
| - Challenge Participants  | |
| - [Tengfei Ma](#tengfei-ma) (IBM) | |
| Workshop Closing  |   |

Please also check out the rest of the [AI Week](https://ibm.biz/ai-research-week) program.


# Keynotes<a name="keynotes"></a>

### Andrew McCallum, UMass Amherst<a name="andrew-mccallum"></a>

*Title*: Embeddings of Language, Knowledge Representation, and Reasoning

### Milind Tambe, Harvard<a name="milind-tambe"></a>

*Title*: AI for Social Good - Learning and Planning in the End-to-End, Data-to-Deployment Pipeline

**Abstract**: With the maturing of AI and multiagent systems research, we have a tremendous opportunity to direct these advances towards addressing complex societal problems. I will focus on the problems of public safety and security, wildlife conservation and public health in low-resource communities, and present research advances in multiagent systems to address one key cross-cutting challenge: how to strategically deploy our limited intervention resources in these problem domains. I will discuss the importance of conducting this research via building the full data to field deployment  end-to-end pipeline rather than just building machine learning or planning components in isolation. Results from our deployments from around the world show concrete improvements over the state of the art. In pushing this research agenda, we believe AI can indeed play an important role in fighting social injustice and improving society.  

### Tim Finin, UMBC<a name="tim-finin"></a>

*Title*: Fifty Years of Using Knowledge Graphs for Language Understanding

**Abstract**: There is a long history of using structured knowledge of one kind or another to support AI tasks and especially ones involving natural language understanding.  Over the years the names and details of changed, from
semantic networks to frames to logic programs to databases to expert
systems to knowledge bases to semantic web and currently to knowledge
graphs.  But a common tread is that an organized representation of
knowledge that can be queried and evolved is a core component of many
intelligent systems. Current research is exploiting today's two big
technology trends: the ready availability of enormous amounts of
content in the form of text, data, images and videos and powerful new
machine learning technologies that can take advantage of it.  After a
brief review of this history, I'll give some examples of combining KR
and ML from our recent work.


# Topical Sessions<a name="topical-sessions"></a>

## L+R Graph Representations

### Brandy Freitas, Pitney Bowes<a name="brandy-freitas"></a>

*Title*: Graph Native Machine Learning

**Abstract**: Graph databases have become much more widely popularized in the recent year. By representing highly connected data in a graph, we have access to a host of graph native algorithms that depend on and exploit the relationships between our data. Computing and storing graph metrics can add strong new features to nodes, creating innovative predictors for machine learning. Using algorithms designed for path finding, centrality, community detection, and graph pattern matching, we can begin to rely less on inflexible, subject-driven feature engineering. In this session, Brandy Freitas will cover the interplay between graph analytics and machine learning, improved feature engineering with graph native algorithms, and outline the current use of graph technology in industry.


### Kelsey Allen, MIT<a name="kelsey-allen"></a>

*Title*: Embodied graph networks - learning graph-based models and policies for physical interaction
 
**Abstract**: Many tasks we care about in the physical environment can be represented as graphs, such as towers of blocks or even more general physical scenes. In this talk, I will describe our ongoing work to learn models and policies which enable artificial agents to build block towers, stabilize block towers with artificial "glue", and perform long-range predictions of complex 2D and 3D shapes in artificial physical environments.

### Ferran Alet, MIT<a name="ferran-alet"></a>

*Title*: Graph Element Networks

**Abstract**: We explore the use of graph neural networks (GNNs) to model spatial processes in which there is no a priori graphical structure. Similar to finite element analysis, we assign nodes of a GNN to spatial locations and use a computational process defined on the graph to model the relationship between an initial function defined over a space and a resulting function in the same space. We use GNNs as a computational substrate, and show that the locations of the nodes in space as well as their connectivity can be optimized to focus on the most complex parts of the space. Moreover, this representational strategy allows the learned input-output relationship to generalize over the size of the underlying space and run the same model at different levels of precision, trading computation for accuracy. We demonstrate this method on a traditional PDE problem, a physical prediction problem from robotics, and learning to predict scene images from novel viewpoints.

## L+R New Combinations

### Masataro Asai, IBM<a name="masataro-asai"></a>

*Title*: Classical Planning in Deep Latent Space: Bridging the Subsymbolic-Symbolic Boundary

**Abstract**: Current domain-independent, classical planners require symbolic models of the problem domain and instance as input, resulting in a knowledge acquisition bottleneck. Meanwhile, although deep learning has achieved significant success in many fields, the knowledge is encoded in a subsymbolic representation which is incompatible with symbolic systems such as planners. We introduce LatPlan, an unsupervised architecture combining deep learning and classical planning. Given only an unlabeled set of image pairs showing a subset of transitions allowed in the environment (training inputs), and a pair of images representing the initial and the goal states (planning inputs), LatPlan finds a plan to the goal state in a symbolic latent space and returns a visualized plan execution.

### Lee Martie, IBM<a name="lee-martie"></a>

*Title*: Reflecting After Learning for Understanding

**Abstract**: Today, image classification is a common way for systems to describe images. While neural network approaches to classification have seen great progress in reducing error rates, it is not clear what this means for a cognitive system needing to make sense of the multiple and competing labels from its own classifiers for image understanding. As a step to address this, we present a novel approach and framework using meta-reasoning and meta-operations to unify labels into higher-level knowledge for the cognitive system. Using our framework on images from ImageNet, we demonstrate systems capable of unifying 41% to 46% of labels and 67% to 75% of labels when these systems can explain their differences. Further, we demonstrate such systems in "the wild" by feeding live video images through one and show the system unifying 51% of labels and 69% of labels when the system can explain their differences. In a survey given to 24 participants, it was found that 87% of the unified labels made with our system describe their corresponding images.


### Lucian Popa, IBM<a name="lucian-popa"></a>

*Title*: Human-Machine Co-Creation of Explainable Models

**Abstract**: While the role of humans is increasingly recognized in machine learning community, representation of and interaction with models in current human-in-the-loop machine learning (HITL-ML) approaches are too low-level and far-removed from human's conceptual models. I will present ongoing work in my team to support human-machine co-creation with learning and human-in-the-loop techniques. In particular, I will focus on HEIDL, a system supports human-machine co-creation by exposing the machine-learned model through high-level, explainable linguistic expressions. In HEIDL, human's role is elevated from simply evaluating model predictions to interpreting and even updating the model logic directly by enabling interaction with rule predicates themselves. Raising the currency of interaction to such semantic levels calls for new interaction paradigms between humans and machines that result in improved productivity for model development process. Moreover, by involving humans in the process, the human-machine co-created models generalize better to unseen data as domain experts are able to instill their expertise by extrapolating from what has been learned by automated algorithms from few labelled data.




## L+R Over Graphs

### Alfio Gliozzo, IBM<a name="alfio-gliozzo"></a>

*Title*: Knowledge Induction @ IBM Research AI

### Ganesh Ramakrishnan, IIT Bombay<a name="ganesh-ramakrishnan"></a>

*Title*: Knowledge Understanding and Representation for Automatic
Question Generation


### Lingfei Wu, IBM<a name="lingfei-wu"></a>

*Title*: Exploiting Graph Neural Networks with Context Information for RDF- to-Text Generation

**Abstract**: The task of RDF-to-Text generation is to generate a corresponding descriptive text given a set of RDF triplets. Most of the previous approaches either cast this task as a sequence- to-sequence problem or employ graph-based encoders for modeling RDF triplets and decode a text sequence. However, none of these methods can explicitly model both global and local structure information within and between the triplets. Furthermore, they did not exploit the target text as an important additional context for modeling complex RDF triplets. To address these issues, we propose to jointly learn local information and global structure information via combining graph encoder and graph-based triple encoder for the input triplets. Furthermore, we also exploit Seq2Seq-based auto-encoder to leverage target text as the context to supervise the combination of input encoders. Experimental results on the WebNLG dataset show that our proposed model outperforms the state-of-the-art baselines.

### Achille Fokoue, IBM<a name="achille-fokoue"></a>

*Title*: TRAIL: A Deep Reinforcement Learning Approach to First-Order Logic Reasoning

**Abstract**: Traditional first-order logic (FOL) reasoning systems usually rely upon manual heuristics to aid in their search for proofs or solutions.  We propose TRAIL: a flexible, deep reinforcement learning based FOL reasoner that circumvents the need for customized heuristics by learning to improve its search and decision-making process. TRAIL relies upon a traditional reasoner and a learning agent that are agnostic of one another, an architecture that allows for developing neural reasoners for any logic. We demonstrate that TRAIL is comparable to state of the art FOL reasoners.

### Tengfei Ma, IBM<a name="tengfei-ma"></a>

*Title*: Graph Enhanced Cross-Domain Text-to-SQL Generation

**Abstract**: Semantic parsing is a fundamental problem in natural language understanding, as it involves the mapping of natural language to structured forms such as executable queries or logic-like knowledge representations. Existing deep learning approaches for semantic parsing have shown promise on a variety of  benchmark data sets, particularly on text-to-SQL parsing. However, most text-to-SQL parsers do not generalize to unseen data sets in different domains. In this paper, we propose a new cross-domain learning scheme to perform text-to-SQL translation and demonstrate its use on Spider, a large-scale cross-domain text-to-SQL data set. We improve upon the SyntaxSQLNet, by constructing a graph of column names for all databases and using graph neural networks to compute their embeddings.  The resulting embeddings offer better cross-domain representations and SQL queries, as evidenced by substantial improvement on the Spider data set.





<!-- # KR2ML Poster Session<a name="poster-session"></a>

## List of Accepted Posters

List TBA<div class="posts-list">
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
