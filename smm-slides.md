Tutorial 6: Social Media Mining in Learning Contexts
========================================================
author: Bodong Chen
date: #LASI2018, June 11-13, NYC
autosize: true



About Me
========================================================

Assistant Professor in learning technologies  
University of Minnesota

- Collaborative learning
- Learning analytics
- MOOCs

Acknowledgements
====

I do not own the copyright of any of the images in this presentation. I therefore acknowledge the original copyright. Other content in this presentation (e.g., text and code) is licensed under a [Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/) license.

<img src="http://www.goopen.no/wp-content/uploads/2016/11/CC-BY_icon.svg_.png" width=400>
<!-- ![](http://www.goopen.no/wp-content/uploads/2016/11/CC-BY_icon.svg_.png) -->

## Disclaimer

Work included in this presentation is produced for teaching purposes only and is hereby not intended for generalizable scholarly knowledge.

Housekeeping
========================================================

- **Github repository**: http://bit.ly/lasi18smm
  - `git clone` or `Download ZIP`
- **Twitter hashtag**: #LASI18smm


Feel free to ask questions ANYTIME!

Prep
====

### Install

1. [R](https://cran.r-project.org/)
2. [RStudio development environment](https://www.rstudio.com/)
3. R packages: `tidyverse`, `igraph`, `sna`, ...
  - [How to install, load, and unload packages in R](http://www.dummies.com/programming/r/how-to-install-load-and-unload-packages-in-r/)

<!-- ### Alternative -->

<!-- - CoLaboratory (check whether R works) -->
<!-- - Watson Studio -->

### Pair-up

![](https://media.giphy.com/media/DohrJX1h2W5RC/giphy.gif)

Tentative Agenda
====

1. Social media basics
2. Social media for learning  
(Short Break)  
3. Collecting social media data
4. Mining social media data

Part 1: Social Media Basics
====
type: section

What are social media?
====

1. Pair & Share  
(self-intro)
2. Tweet out your definition(s) -- [#LASI18smm](https://twitter.com/search?q=%23LASI18smm&src=typd)

![](smm-slides-figure/twitter-hashtag.png)


What do social media researchers say?
====

Gruzd, Staves, & Wilk 2012:

![](smm-slides-figure/gruzd2012.png)

<!-- Examples of social media include social network sites (e.g., Facebook); wikis (e.g., wikispaces); media-sharing services (e.g., YouTube); blogging tools (e.g., Blogger); micro-blogging services (e.g., Twitter); social bookmarking (e.g., Delicious); bibliographic management tools (e.g., Zotero); and presentation-sharing tools (e.g., Slideshare). -->


What do social media researchers say?
====

Obar & Wildman, 2015:

1. Social media services are (currently) Web 2.0 Internet-based applications
2. User-generated content is the lifeblood of social media
3. Individuals and groups create user-specific profiles for a site or app designed and maintained by a social media service
4. Social media services facilitate the development of social networks online by connecting a profile with those of other individuals and/or groups

Example: Twitter
====

![](https://i0.wp.com/www.mattberinger.com/wp-content/uploads/2017/09/tweet-anatomy-for-my-article-SAVED-FOR-WEB.png?resize=1181%2C502)

Example: Twitter
====

![](smm-slides-figure/goggins-twitter.png)

(Goggins & Petakovic, 2014)

Example: Github
====

![](https://answers.unrealengine.com/storage/temp/56639-git.png)

Example: Github
====

![](smm-slides-figure/goggins-github.png)

(Goggins & Petakovic, 2014)

Example: Wiki
====

<img src="https://upload.wikimedia.org/wikipedia/commons/3/34/Wikimedia_logo_family_complete_2.svg" width=600px>

<!-- ![](https://upload.wikimedia.org/wikipedia/commons/3/34/Wikimedia_logo_family_complete_2.svg) -->

Part 2: Social Media for Learning
====
type: section

AND  
Learning on Social Media

Educational Affordances
====

- connectivity (interconnections)
- interactivity
- information sharing and discovery
- content creation, remixing
- etc.

(Bates; Greenhow; Siemens & Downes)

Cases
====

1. Pair & Share
  - What educational use of social media you're involved/interested in?
  - How is *learning* conceptualized in the context?

Learning attributes on social media
====

INSERT TABLE HERE

(Adapted from Greenhow & Lewin, 2016)


Broadening the Conceptualization & Scope
====

Learner-centered themes

- Learners' participation and creative practices
- Learners' online identity formation

(Greenhow et al., 2009)



Influence, Participation and Affiliation
====

![](smm-slides-figure/goggins-table.png)

(Goggins & Petakovic, 2014)

Social (and Socialized) Learning
====

![](smm-slides-figure/buckingham-shum.png)

(Buckingham Shum & Ferguson, 2012)

Context Matters!
====

Example: [CCK08 cMOOC](https://www.slideshare.net/gsiemens/moocs-educause), Siemens

![](https://image.slidesharecdn.com/moocseducause-120731102926-phpapp02/95/moocs-educause-14-728.jpg?cb=1343730651)

Example: Open Learning MOOC
====

http://openlearninghub.net/ (Garnder Campbell)

![](smm-slides-figure/open-learning.png)

Example: Open Learning MOOC
====

[Twitter conversations](https://hawksey.info/tagsexplorer/?key=1HnD3t0x9kSfRiqRvUknHIQDQuxwXjH93eEbo4NsVjFU&gid=400689247)


Example: Connected Learning
====

![](https://clalliance.org/wp-content/themes/cla2016/images/Graphic-Main-2.png)

Example: Connected Learning
====

![](https://clalliance.org/wp-content/themes/cla2016/images/Graphic-Main-2.png)

<!-- a social MOOC (https://www.futurelearn.com/courses/social-media-analytics?utm_campaign=Share+Links&utm_medium=futurelearn-run_details&utm_source=twitter#section-educators) -->

Example: Connected Learning
====

![](http://lt.umn.edu/news/wp-content/uploads/2015/12/scigirls-pbs-kids-header21.png)

Example: Personal Learning Networks
====

\#personalizedpd

<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">Welcome to <a href="https://twitter.com/hashtag/personalizedPD?src=hash&amp;ref_src=twsrc%5Etfw">#personalizedPD</a> Introduce yourself and one word or phrase that has described your school year? <a href="https://twitter.com/hashtag/personalizedPD?src=hash&amp;ref_src=twsrc%5Etfw">#personalizedPD</a> <a href="https://t.co/asgeckhZPL">pic.twitter.com/asgeckhZPL</a></p>&mdash; Heidi Carr (@carr_8) <a href="https://twitter.com/carr_8/status/1004166232080289792?ref_src=twsrc%5Etfw">June 6, 2018</a></blockquote>
<script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>


Example: #MarginalSyllabus
====

"The Marginal Syllabus convenes and sustains conversations with educators about issues of equity in teaching, learning, and education."

![](http://marginalsyllab.us/wp-content/uploads/2017/08/cropped-header-aug17.jpeg)



<!-- Annotation communities - Climate Feedback -->

Example: Scholarly Communication
====

![](https://www.researchgate.net/profile/Wanli_Xing2/publication/323839719/figure/fig3/AS:614032633507845@1523408196237/The-largest-connected-interaction-network-components-from-LAK11-to-LAK14-Note-Node-size.ppm)


Open Discussion
====
type: prompt



Part 3: Collecting Social Media Data
====
type: section


Research Ethics
====
type: prompt

- Research
- Human subjects
- Private information
- Informed consent
- ...



Case Study 1: #personalizedpd
====

<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">Join me on the <a href="https://twitter.com/hashtag/PersonalizedPD?src=hash&amp;ref_src=twsrc%5Etfw">#PersonalizedPD</a> chat tomorrow for a special discussion on <a href="https://twitter.com/hashtag/MergeCube?src=hash&amp;ref_src=twsrc%5Etfw">#MergeCube</a> resources! <a href="https://twitter.com/hashtag/ARVRinEDU?src=hash&amp;ref_src=twsrc%5Etfw">#ARVRinEDU</a> <a href="https://twitter.com/hashtag/edtech?src=hash&amp;ref_src=twsrc%5Etfw">#edtech</a> <a href="https://twitter.com/MergeVR?ref_src=twsrc%5Etfw">@MergeVR</a> <a href="https://t.co/PIbZPhUqKA">pic.twitter.com/PIbZPhUqKA</a></p>&mdash; Jaime Donally (@JaimeDonally) <a href="https://twitter.com/JaimeDonally/status/988401616058544128?ref_src=twsrc%5Etfw">April 23, 2018</a></blockquote>
<script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

Case 1: #personalizedpd
====

Blog posts

> At first Twitter allowed me to fill the personalized PD void and connected me with others who both challenged my thinking and inspired me to be a better educator than I was. ...
>
> Then, one glorious day, I found the #personalizedPD chat and my entire perspective changed. Instantly, I loved these people.
>
> -- [Mandy Froehlich](https://mandyfroehlich.com/2016/04/20/i-just-met-you-but-i-love-you/)

Collect Tweets
====

TAGS
- https://tags.hawksey.info/
- Collect (Twitter API key needed)
- Publish

![](https://tags.hawksey.info/wp-content/uploads/2014/09/cropped-TAGSLogo2.png)

<!-- - https://mashe.hawksey.info/2011/11/twitter-how-to-archive-event-hashtags-and-visualize-conversation/ -->


Collect Tweets
====


```r
# Load helpful functions written by Bodong
source("utils/collect_tweets.R")
source("utils/munge_tweets.R")

# URL to the published sheet
gsheet_url <- "https://docs.google.com/spreadsheets/d/e/2PACX-1vRzuK4ltTt6jSJXYAhj-ERxvlhw3UsP5zCeCyrfXfEwNyTRu8kn_Hn8RwVewaxMPly2KcJAiciCTK_0/pub?gid=400689247&single=true&output=csv"

# Collect tweets archived in the sheet
tweets_raw <- collect_tweets_from_gdrive(gsheet_url)
```

Clean and store data
====


```r
# basic data cleanup (incl. removing duplicates)
tweets <- preprocess_tweets(tweets_raw)

# save cleaned data as a csv file
write_csv(tweets, path = "data/tweets.csv")
```


Case 2: #MarginalSyllabus
====

![](smm-slides-figure/marginalsyllabus.png)


Collect Hypothesis Annotations
====

API (aka. Application Programming Interface)


```r
# Load helpful functions written by Bodong
source("utils/collect_annotations.R")

# Collect annotations
annotations <- collect_annotations(tag = "marginalsyllabus",
                                   token = h_token,
                                   num = 500)
```

Store data
====


```r
# save data as an Rdata file
save(annotations, file="data/annotations_raw.Rdata")
```


Storing data
====

Porpular formats
- CSV (comma-separated vectors)
- JSON
- Relational databses (e.g., MySQL)
- GraphDB (e.g., Neo4j)
- ...

Neo4j
====

![](smm-slides-figure/neo4j-eg.png)


Troubleshooting?
====
type: prompt



Part 4: Mining Social Media Data
====
type: section


Mining what?
====
type: shoutout

Connectivity of a community
====



Influence and leadership
====


Community evolution
====

Cognitive and affective states
====

Q & A
====
type: section
