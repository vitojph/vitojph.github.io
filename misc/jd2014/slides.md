## Interaction Design for Multilingual Information Access beyond Document Retrieval

<br/>
<br/>

ETSI Informática, UNED | 9/06/2014

Víctor Peinado | victor@lsi.uned.es | @vitojph  


--SLIDE--
### Outline

1. [Motivation](./#/2)

2. [Goals](./#/3)

3. [Hypothesis](./#/4)

4. [Methodology](./#/5)

5. [Work in progress](./#/6)


--SLIDE--
### Motivation

- As the number of Internet users grows, more non-English speakers have access to the Web.

- The language gap is the first barrier and MLIA technology can facilitate accessing, querying and retrieving information from multiple sources and across languages.

- Searching for information is an eminently interactive process, but advances achieved in automatic IR have not yet been proved successful with real users.

- How can we properly assist people to find and use information expressed in unknown languages?



--SLIDE--
### Goals

<br/>

- To study and understand how the change from a monolingual to a multilingual environment modifies people’s performance, behavior and satisfaction when searching for information.

--SUBSLIDE--
### Interactive document retrieval is not a complete task

<br/>

- how many documents chosen by the user are relevant for the query? but;

- we cannot confirm that users were actually able to fulfill the initial information need

--SUBSLIDE--
### Beyond document retrieval

<br/>

- **interactive question answering**

  - brief passages vs. full documents
  - pre-specifying the expected type of answer can help users?
  - automatic highlighting of the possible target answers is useful?

--SUBSLIDE--

- **interactive image search**

  - are users willing to translate into unknown languages?
  - competence in target language determines the success of the task?
  - actual usage of CL facilities vs. users' perception of usefulness

--SUBSLIDE--

<br/>

The conclusions of these analyses will allow us to propose mechanisms, tools and good practices to better assist users when searching for information in unknown languages.


--SLIDE--
### Hypothesis

- In monolingual information access tasks user’s intelligence compensates for system’s lacks.

- A user can easily learn how to use information retrieval’s interactive functionalities.

- In a CL environment, the user cannot adapt herself to a new language.

- Unable to search in unknown languages unless CL functionalities are provided by the system.

--SUBSLIDE--

### Hypothesis

<br/>

- in interactive cross-lingual information access tasks, the **cross-language facilities are the key factor** to explain people’s performance, behavior and experience.


--SLIDE--
### Methodology

- Conduct interactive QA experiments in a controlled CL scenario to provide evidence about the difficulties of searching answers.

- Test the usefulness of different access methods and search functionalities:

  - passages vs. documents.
  - automatic highlighting of potential expected answers.

--SUBSLIDE--

- Conduct interactive search experiments in a naturally multilingual images database: Flickr.

  - User-centered experiments in laboratory conditions aimed to test how CL technologies could enhance access

  - Explore the user interaction resulting from this.

--SUBSLIDE--

- Propose an image search task as a game.

  - Design a transaction log to capture every single detail of the multilingual
image search process.

  - Build a multilingual search interface for Flickr, supporting the collection of a medium size search log of multilingual image searches.

  - Apply transaction log analysis to understan the complete multilingual search processes from a user’s perspective.


--SLIDE--

### Work in progress

<br/>

Users’ Perceptions, Search Behavior and Search Effectiveness in Interactive Multilingual Search

--SLIDE--
### Outline

1. [Experimental Design: FlickLing and iCLEF](./#/8)

2. [Method of Analysis](./#/9)

3. [Performance](./#/11)

4. [Effort](./#/12)

5. [Usage of CL Facilities](./#/13)

6. [Users' Perceptions](./#/14)

7. [Conclusions](./#/15)

8. [Chronogram & To-Do List](./#/16)

--SLIDE--

### Experimental Design

--SUBSLIDE--

### FlickLing and iCLEF

- FlickLing: a multilingual search interface for Flickr (Peinado et al., 2008) is the multilingual search interface provided by iCLEF organizers.

- Designed to collect a large search log of multilingual image searches

- Two interfaces to perform monolingual and multilingual searches over the Flickr database, retrieving images annotated in different languages.

- Proposed as a competitive game.

--SUBSLIDE--

### Monolingual interface

<br/>

![](img/mono-interface-en.png)

--SUBSLIDE--

### Cross-language interface

<br/>

![](img/cl-interface-en.png)


--SUBSLIDE--

### Customized dictionary

<br/>

![](img/add-translations-en.png)


--SUBSLIDE--

### Ranking of results for the query *santa monica pier*

![](img/ranking-en.png)

--SUBSLIDE--

### RF functionalities

<br/>

![](img/search-from-tag-en.png)

--SUBSLIDE--

### Search sessions

<br/>

- Users were given raw images as target: images were chosen randomly from the pool.

- Users could launch monolingual and multilingual searches, manipulating the automatic translations or refining their queries.

- When a user found the target image, she obtained 25 points.

--SUBSLIDE--

- At any time, users could stop searching and quit.

  - Then, the system offered some hints.
  - If the hint was accepted, the score was penalized for 5 points.

- The session finished when the user either found an image or gave up.

- The game could last as long as it has to but, internally, the experiment was considered as finished after 15 sessions.


--SUBSLIDE--
### Questionnaires

1. post-image questionnaire about the easiness or difficulty of the task, depending on the outcome of the search session

2. after 15 search sessions, extensive details about:
   - user's background and previous experience searching information in foreign languages
   - how clear, easy, familiar, interesting and relevant the task had been
   - the most challenging aspects of the task
   - usefulness of the interface’s facilities
   - any other missing functionalities
   - strategies used to find the correct translations

--SLIDE--

### Method of Analysis

--SUBSLIDE--
### Log Analysis

- The logs collected and released during the iCLEF 2008 and 2009 campaigns contained more than 2M lines.

- Some users:
   - registered and tried out just a few searches.
   - were caught cheating.
   - were wrongly captured in the logs and considered invalid.

- We restrict the analysis to the **3,025 individual search sessions** carried out by users who were able to complete at least 15 search sessions.

--SUBSLIDE--
### 3 independent variables

<br/>

- **user profile**: active (N=1,882) / passive (N=442) / none (N=701)
  - according to the users' language skills wrt the language of the target image.

- **difficulty** of the target image: easy (N=1521)/ difficult (N=1461)
  - *easy* images are those with higher avg success rate (threshold = 79%)

- **number of search session** [1:15]
  - is there any type of learning effect?

--SUBSLIDE--
### 4 dependent variables

<br/>

- **result** of the search session :-) or :-(

- **score**: points obtained in the search session [0:25]

- **hints** requested [0:5]

- **# interactions**: user's total effort in performing the task (queries launched, ranking pages explored, usage of RF facilities

--SLIDE--

### Results

--SLIDE--

### Performance


--SUBSLIDE--
### Performance per user profile

![](img/histograms-performance-profile.jpg)

--SUBSLIDE--
### Performance thru time

![](img/plot-performance-15.jpg)

--SLIDE--

### Effort

--SUBSLIDE--
### Interactions as a proxy of users' effort

<br/>

<table class="reveal">
    <tr>
      <th>user profile</th>
      <th>mean</th>
      <th>SD</th>
    </tr>
    <tr>
      <td>active</td>
      <td>11.27</td>
      <td>13.66</td>
    </tr>
  <tr>
    <td>passive</td>
    <td>12.48</td>
    <td>16.07</td>
  </tr>

  <tr>
    <td>none</td>
    <td>12.83</td>
    <td>14.98</td>
  </tr>
  </table>

<br/>

- These differences are only significant in the active-none comparison (p < 0.04)

--SUBSLIDE--
### Lack of language skills &rarr; more effort

![](img/effort-table.png)

- the lack of language skills seems to be directly related to:
  - the usage of the multilingual search mode
  - the total number of interactions performed.


--SUBSLIDE--
### Interactions decrease thru time

<br/>

![](img/plot-median-interactions15.jpg)

--SUBSLIDE--
### Effort wrt difficulty of the target image

![](img/histograms-interactions-difficulty-images.jpg)

--SUBSLIDE--

![](img/histograms-loginteractions-difficulty-images.jpg)

- Differences between these two groups are significant (p < 0.0005)

--SLIDE--

### CL facilities

--SUBSLIDE--
### Usage of the CL facilities is very low

<br/>

<table class="reveal">
    <tr>
      <th>user profile</th>
      <th>mean</th>
      <th>SD</th>
    </tr>
    <tr>
      <td>active</td>
      <td>0.06</td>
      <td>0.45</td>
    </tr>
  <tr>
    <td>passive</td>
    <td>0.06</td>
    <td>0.43</td>
  </tr>

  <tr>
    <td>none</td>
    <td>0.17</td>
    <td>0.79</td>
  </tr>
  </table>

<br/>

- only 40% of users employed either the multilingual RF or their personal dictionary

- dictionary manipulation is the most frequently used

--SUBSLIDE--
### CL facilities don't decrease thru time

<br/>

![](img/RF15.png)

<br/>

- personal dictionary turned out to be more useful as users were completing search sessions.


--SLIDE--

### Users' Perceptions

--SUBSLIDE--

### It's an easy task but...

<br/>

![](img/post-image-quest-success.jpg)

- to describe the image and the language barrier are the main difficulties

--SUBSLIDE--

### Users quit because...

<br/>

![](img/post-image-quest-fail.jpg)

- too many images to deal with
- it's difficult to describe the image


--SUBSLIDE--

### Most challenging aspects of the task

![](img/oq-challenging-aspects.png)

--SUBSLIDE--

### Selecting the best translations

![](img/oq-how-select-best-translations.png)


--SUBSLIDE--

### Most useful interface’s facilities

![](img/oq-useful-facilities.png)

--SUBSLIDE--

### Missed any other facilities?

![](img/oq-facilities-missed.png)

--SLIDE--


### Conclusions

--SUBSLIDE--

### Conclusions

- performance of users with passive competence in the target language is similar to users’ with active competence, but at the expense of employing more effort.

- users with no competence in the target language obtain poorer results.

- the language barrier is perceived as the most challenging aspect of the task.

--SUBSLIDE--

- users resist to use multilingual search assistance, even when they find out they have to search in unfamiliar languages.

- CL facilities are scarcely used but they are the only functionality whose usage does not decrease across time, they are used more frequently than standard RF features.

- CL facilities are highly appreciated by users.

--SLIDE--

### Chronogram

--SUBSLIDE--

### Objectives partially achieved

- Passages preferred over documents, but documents are more effective  (López-Ostenero et al., 2005; Peinado et al., 2006; López Ostenero et al., 2008).

- Specifying the expected type of answer before launching the query is helpful (López-Ostenero et al., 2005).

- Automatic highlighting of the possible target answers is useful (Peinado et al., 2006).

--SUBSLIDE--

- Users tend to avoid translating their queries and search for images tagged in unknown languages: (Artiles et al., 2009).

- User with active competence in the target language perform 18% better than users with no competence (Peinado et al., 2009a,b)

- Users with passive competence need more interactions (Peinado et al., 2009a,b).

--SUBSLIDE--

- Usage of CL facilities is low but higher than RF and is perceived as useful (Artiles et al., 2009; Peinado et al., 2009a,b).

- Usage of RF is remarkably low but successful users use it more often (Artiles et al., 2009; Peinado et al., 2009a,b).

- Re-usable resources: the [iCLEF search log](https://github.com/vitojph/iclef) (Peinado et al., 2008, 2009a,b).

--SUBSLIDE--

### To-do List

- Jun 2014: analyze subjects' performance and effort considering their linguistic competence with respect to the annotation language of the target image.

- Jun 2014: analyze users' perception on the task performed.

- Jun 2014: study users' behavior with respect to the search mode used (monolingual or multilingual).

- Jun 2014: compare usage and usefulness of the different cross-language interactive search facilities implemented in our image search assistant.

- Jul-Aug 2014: write journal article with the latest analyses.

- Sep-Dec 2014: write the dissertation.




--SLIDE--

### Questions?

<br/>
<br/>

Thank you!

--SLIDE--

### Other pending analyses

- width vs depth search

- before and after 1st hint

- hints vs no hints
