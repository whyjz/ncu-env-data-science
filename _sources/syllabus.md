# Syllabus 

**RS5046/GP5024: Environmental data science (環境資料科學)** Spring 2026

Whyjay Zheng (鄭懷傑), whyjz@csrsr.ncu.edu.tw, Tuesday 10:00 am -- 12:30 pm at S-114 (科學一館/地球科學系系館; Department of Earth Sciences)


## Course Goals

- Familiarize yourself with the language data scientists use to communicate. 
- Understand some of the most popular statistical models in environmental science.
- Develop skills to process real data and gain insights.
- Collaborate with your teammates on a big data science project.

## Prerequisites 

Before taking this course, you should already have the necessary knowledge about statistics and computer programming. Check out [this web page](https://scikit-learn.org/1.1/tutorial/statistical_inference/supervised_learning.html) and see if you can understand most of the ideas and steps presented here within a reasonable reading time. 

If more than two questions in the Pre-course Quiz are challenging, I suggest taking introductory statistics or programming first.

## Textbook

Hsieh, W. (2023). Introduction to Environmental Data Science. Cambridge: Cambridge University Press. doi:[10.1017/9781107588493](https://doi.org/10.1017/9781107588493) (PDF available through the [NCU library](https://ncu.primo.exlibrisgroup.com/discovery/search?selection=any,contains,&query=any,contains,Introduction%20to%20Environmental%20Data%20Science&tab=nculib&search_scope=MyInstitution&vid=886UST_NCU:886UST_NCU&lang=zh-tw&offset=0))

## Course Calendar 

Readings and assignments are due **before the class starts**.

```{list-table}
:header-rows: 1

* - Week #
  - Topics
  - Readings due
  - Assignments due
* - 1 (2/24)
  - Syllabus and warm-up | Pre-course Quiz
  - 
  - 
* - 2 (3/3)
  - Linear Models and Regularization (I)
  - 2.11, 5.1, 5.2, 5.5
  -
* - 3 (3/10)
  - Linear Models and Regularization (II) 
  - 2.12, 2.13, 5.6--5.10
  -
* - 4 (3/17)
  - Neural Networks (I)
  - 6.1--6.5
  - Problem set #1
* - 5 (3/24)
  - Neural Networks (II)
  - 7.1--7.6, 7.8
  - 
* - 6 (3/31)
  - *NO CLASS*
  - 
  - Term project proposal  
* - 7 (4/7)
  - *NO CLASS*
  - 
  - 
* - 8 (4/14)
  - Neural Networks (III)
  - 8.1--8.8
  - 
* - 9 (4/21)
  - Principal Components (I)
  - TBD
  - Problem set #2  
* - 10 (4/28)
  - Principal Components (II)
  - TBD
  - 
* - 11 (5/5)
  - Kernel Methods (I)
  - TBD
  - Problem set #3
* - 12 (5/12)
  - Kernel Methods (II)
  - TBD
  - 
* - 13 (5/19)
  - Ensemble Methods (I)
  - TBD
  - Problem set #4
* - 14 (5/26)
  - *NO CLASS*
  - 
  - 
  - Term project paper
* - 15 (6/2)
  - Ensemble Methods (II)
  - TBD
  - 
* - 16 (6/9)
  - Term project presentation | Post-course Quiz
  -
  - Problem set #5 
```
<!-- [2.14--2.16 12.1--12.3, 13.1--13.5]
[13.6--13.8]
[2.17, 14.1, 14.2]
[14.3, 16.8, 16.9, 17.2] -->

<!-- 15.1--15.3 -->
<!-- Outlook: Physics-informed learning models -->
<!-- 
* - Week #
  - Topics
  - Readings due
  - Assignments due
* - 1 (2/18)
  - *NO CLASS*
  - 
  - 
* - 2 (2/25)
  - Syllabus and warm-up | Pre-course Quiz
  - 
  -
* - 3 (3/4)
  - Statistical Tests (I)
  - 4.1--4.5, 4.8
  -
* - 4 (3/11)
  - Statistical Tests (II)
  - 2.11, 5.1, 5.2, 5.5
  - Problem set #1
* - 5 (3/18)
  - Linear Models and Regularization (I)
  - 2.12, 2.13, 5.6--5.10
  - 
* - 6 (3/25)
  - *NO CLASS*
  - 
  - 
* - 7 (4/1)
  - Linear Models and Regularization (II) 
  - 6.1--6.4, 7.1, 7.2
  - 
* - 8 (4/8)
  - Neural Networks (I)
  - 7.3--7.6, 8.1--8.6
  - Problem set #2  
* - 9 (4/15)
  - Neural Networks (II)
  - 2.14--2.16, 6.5, 6.8, 8.7, 8.8
  - Term project proposal  
* - 10 (4/22)
  - Neural Networks (III)
  - 12.1--12.3, 13.1--13.5
  - Problem set #3
* - 11 (4/29)
  - *NO CLASS*
  - 
  - 
* - 12 (5/6)
  - Kernel Methods (I)
  - 13.6--13.8
  - 
* - 13 (5/13)
  - Kernel Methods (II)
  - 15.1--15.3
  - 
* - 14 (5/20)
  - Ensemble Methods (I)
  - 2.17, 14.1, 14.2
  - Problem set #4
* - 15 (5/27)
  - Ensemble Methods (II)
  - 14.3, 16.8, 16.9, 17.2
  - 
* - 16 (6/3)
  - Term project presentation | Post-course Quiz
  -
  - Problem set #5
* - 17 (6/10)
  - *NO CLASS*
  - 
  - Term project paper
* - 18 (6/17)
  - *NO CLASS*
  - 
  -  -->

This tentative schedule is subject to change depending on our progress and participants' needs.

## Course components

### Readings
The assigned readings are from Hsieh's book (see Course Calendar for the section numbers). We will have you discuss your reflection and understanding of the content during the class.

### During the class
There are two segments during the class time:

1. Group discussion (10:00--10:40): You will have to find solutions or perspectives to my questions on a worksheet as a group of 2--3 people. These questions are related to the assigned readings.
2. Lecture (10:45--12:20; with a break of 10 minutes in the middle): I (Whyjay) will review today's topics. We will also use this time to discuss your homework and demonstrate data-processing skills.

### Homework assignments
There will be five problem sets throughout the semester. Each consists of 3--5 questions, most of which (as well as the source data sets) come from Hsieh's textbook. You must work on them individually (no collaboration or plagiarism). Assignments are **due before class starts**; see course calendar for due dates. Electronic submission through ee-class is recommended, but other forms are also acceptable. Please make sure I get your submission before the deadline to avoid a potential late penalty if you don't use ee-class.

### Term project
The group-based term project is the final checkpoint for what you have learned in this course. Each project team consists of no more than four people. There are three project milestones throughout the semester: 

1. A project proposal.
2. An online webpage showcasing the final work of the project.
3. An in-class oral presentation about your work.

All due dates have been listed in the course calendar. For the written submission, the due time is always 10:00 am (i.e., **before the class starts**).  

#### Project proposal

The project proposal should be half to one page long and summarize your intended goals. The goals must be related to multiple topics we cover in the course.

#### Online webpage

Your final group write-up must follow the structure of an academic essay (Introduction, Methods, Results, Discussion, References, etc.) and have an abstract of less than 100 words. The work should be visible online before the due date listed on the calendar (before the class starts) and remain unchanged for a week for grading. After one week, you can decide whether to keep the webpage online.

There will be a template for you to develop your own writing.

<!-- I have made a [template](https://github.com/whyjz/ncu-env-data-science-template) for you to automatically publish your Jupyer notebook (or plain markdown files) using GitHub Pages. You can also find the deployed [HTML here](https://whyjz.github.io/ncu-env-data-science-template/project.html).  -->

#### Oral presentation

A seminar-style presentation summarizing your final project work. The presentation should be with visual aids (slides, media, whiteboard, etc.), in English, and within 20--30 minutes, followed by a Q&A session. Each group member should speak up during the talk. 


## Grading
I will evaluate your submissions and post your grades using Ee-class. The grade breakdown is as follows:

- Readings and class discussion (22％): Each group worksheet accounts for 2% of the grade. I grade it using a simple rubric system: Good (2%), Fair (1%), and Absent (0%). All group members receive the same grade. We expect to receive eleven worksheets this semester. 

- Assignments (50％): Each problem set accounts for 12.5% of the grade. The lowest-graded one will be dropped for final grade calculation. Most of the problems are from Hsieh's book, which provides the suggested solution for some questions. But remember: **The doing is often more important than the outcome.** The grades of your assignments are heavily based on the reproducibility of your workflow (8.75%) rather than the correctness of your results (3.75%). Please include scripts, screenshots, or other elements that allow others to reproduce your work. 

- Term project (30％): Project proposal accounts for 5%. I will typically give you full credit for this unless it does not meet the formatting requirements. The written webpage accounts for 10%, and the final oral presentation accounts for 15%. These are graded based on work quality, completeness, clarity of the presentation, and the ease with which others can reuse your workflow or results. All team members receive the same base grade as above, plus individual grade adjustments based on a confidential poll of teammates.

The sum of these grading items is 102%; however, you will receive 100% if your total is over 100%. 
 

(late-work-policy)=
### Late work policy
- Write-ups: A 10% penalty will be applied for each day past the deadline. 
- Term project presentation: If you are absent on the oral presentation date, we accept video recordings to be shared within the class as a make-up. However, a 20% penalty will be applied for each day past the presentation date. 
- With reasonable proof, the policies above may be exempted under particular circumstances, such as family emergencies or urgent medical conditions. Please let me know (Whyjay) as soon as possible if this happens so we can discuss make-up plans as needed.


## Code of conduct

### Diversity, Equity, and Inclusion (DEI)

- We will not tolerate any forms of discrimination and harassment during the class. 

- We encourage conversations about inequality whenever you sense that. This includes, but is not limited to, the [hidden curriculum](https://en.wikipedia.org/wiki/Hidden_curriculum) and [microaggression](https://en.wikipedia.org/wiki/Microaggression). 

- Be respectful about different ideas and perspectives during discussion, and be mindful about your choice of words. 

### Attribution of work

- Please be careful about using copyrighted material in any assignments, and **make sure you have permission/license with proper attribution** whenever you use it.

- Again, do not work with other students on the homework assignments. They must be your sole work.

### Study time
Since this is a 3-credit course, I expect you to have ~6 hours of study time each week in addition to class time to earn an adequate grade. If you spend much less or much more than that on readings, assignments, and the project, please let me know.

### AI policy
Generative AI is allowed and encouraged (HEY... this is the power of data science!!). Use it with discretion, though -- generative AI is **good at popular tasks** (such as generating code to visualize a typical data structure) but **not good at generating ideas and perspectives**. Their answers are usually very dull (if not failing a sanity check) due to the nature of the training process.

### Working languages
We use English as the primary language for communication during class and the oral presentation. There is an exception, though: you can use a different language in a group discussion if everyone agrees. 

All writing assignments and reports must be prepared in English.

You are welcome to complete assignments using any programming language. I am familiar with Python and Matlab, and can comment more if you use either. We will use Python with the Jupyter ecosystem (including Colab) for the class demos.

### Auditing 

Auditing is welcome. If you plan to audit the course, please note:

- You cannot submit assignments or join any term project teams. 
- You can join any group during the in-class discussion time as long as all the group members agree.

<!-- Other topics in data science (such as principal component and clustering analysis) will be covered through assigned readings, which we rely on during the class discussion. -->

<!-- 
Part 2
Regression Models: Why is regularization so important? (Weeks 4-6)
Part 3
Neural Networks: How to trust deep models that seem like black boxes? (Weeks 7-9)
Part 4
Kernel Methods: Is dimensionality a curse or a blessing? (Weeks 10-12)
Part 5
Random Forests: When one model is not enough, make several? (Weeks 13-15)
Part 6
Final hacker group presentation (Week 16) -->

<!-- 
Unnecessary:
2025: Inference x2, ensemble models,

Needs to be extended:
2025: NN + RF, all non-linear models, RF, NN, kernel models 
2025-zh: kernel models

Future directions:
2025: Markov models x2, TS models x2, cluster analysis x2, preprocessing
2025-zh: ensemble models, cluster analysis

Suggestions:
2025: discuss homework, more relevant homework, start project early, code implementation
2025-zh: inference is a must have
-->