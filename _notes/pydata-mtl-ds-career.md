---
layout: page
title: Notes | PyData Montreal- Building your Data Science Career
---

_Panelists_: [Vicki Boykis](https://twitter.com/vboykis), [Alexey Grigorev](https://twitter.com/Al_Grigor), [Emily Robinson](https://twitter.com/robinson_es)

_Hosts_: Maria Khalusova and Alex Kim

_Links: [Meetup](https://www.meetup.com/PyData-MTL/events/270416417), [Youtube](https://youtu.be/YowjjiSSq54)_

_Note: The notes here are not exactly chronological. I have tried to group them together as I see fit_. 

## Getting into Data Science

### How is Data Science now?
- _[V]_ The field is very big now. To stand out, one good way is to learn software engineering. Also, could start from an adjacent position and move sideways. 

   Ref: [Data Science is Different Now](http://veekaybee.github.io/2019/02/13/data-science-is-different/)

- _[V]_ Also, there are tiers of company that have different requirements/expectations from Data Scientists.
- _[E]_ There are still a lot of low-hanging fruits. Don't have to do cutting-edge stuff.
- _[E]_ Don't need to worry about the title. "Anything that gets you working with data is valuable experience".
- _[A]_ The focus is now on engineering too, which people have realized is important for the business. One example: not as many jobs listing a PhD as a requirement.

### What common advice is counterproductive?
- _[E]_ "You need to learn X / do Y to be a Data Scientist". This is just Gatekeeping.
    - Instead, realize that the role is different for different jobs/companies. 
    A Data Scientist may excel in a particular setting/company but may find it difficult in another company.  

### What to do to get into DS in the next two years? What has the biggest ROI?
- _[E]_ Don't get a PhD just for the sake of getting into DS
- _[E]_ Learning on the job is good. You don't have to know _everything_ before getting into the field.
- _[V]_ Books and learning on the job are good.
- _[V]_ Do projects to show knowledge and skills. What companies want is someone who can hit the ground running. 
- _[A]_ Kaggle. It teaches you things like choosing the validation setup, and a whole bag of tricks and tips. 
- _[E]_ Complement Kaggle with a problem of your own formulation  


### How do you keep up? How do you prioritize what you learn?
- _[A]_ Learn the fundamentals and the underlying principle. E.g: Distributed Systems when learning Kubernetes.
- _[V]_ "Wait for the dust settle in". You don't have to jump right into the newest shiny thing.  


### Making the transition from Software Engineering to Data Science _[A]_
- A lot of what you already know helps.
- Major Obstacle?
    - Too much information. To solve this, have a problem in mind and learn what's necessary for that.  


### Project Manager to Data Scientist
- _[A]_ Learn Coding. Pick up Python. 
- _[E]_ There are already some parts of the role amenable to being molded into analysis of data. Can look to use Looker or Tableau and then use Python for the same. Also good to note that a lot of the other transferable skills can be helpful: communication, handling multiple stakeholders, thinking in terms of products.  


## Job Applications

### Job titles under the DS umbrella _[V]_
- Data Scientist: the most generalist now.
- Machine Learning Engineer: expected to know how to build the pipelines end-to-end.
- Research Scientists: Deep work in algorithms.
- Data Analyst (but now termed Data Scientist): The "traditional" analyst role.

### DS Roles _[E]_  

Ref: [Red flags in Data Science Interviews](https://hookedondata.org/red-flags-in-data-science-interviews/)

- Not exactly red flags but do factor in that there is a lot of difference based on preference. 
    - E.g. Do you want to be the first on the DS team or need a DS team already there?
    - Startup vs big company? How okay are you with bureaucracy?

How to get noticed in a job application?
- _[V]_ Have a warm connection with someone in the company. Network. One way could be to put out a blog and interact with the wider community. Could even DM the hiring manager if they are open to it. 
- _[V]_ Do projects that are complete and annotated. There are a lot of DS content out there but not that many good content.
- _[E]_ Organize your projects. Have a good README. Have some sort of product at the end. Could be a Dashboard, blog post, or an interface.
- _[E]_ "Don't be afraid to show your personality". Narrow down what you need to learn to work towards solving a problem.

How to get better at technical writing?
- _[V]_ Be consistent. Have a small group of people who give good feedback. A blog shows the day-to-day of how the person thinks.

What to expect in a job application process?
- _[A]_ One could be: Phone screening, home assignment, assignment defense, behavioral interviews, and so on, depending on the job level.
- _[V]_ Ask the Hiring manager because it can be a lot of different things.
- _[E]_ Reminder: Don't be too hard on yourself. It could be a position that's not a good fit rather than something being wrong with you.
- Home Assignments
    - _[A]_ If you don't agree, one good response might be: "I don't accept it, but _this_ is how I would solve it. Here's some code of mine and blog posts to show how I think. I would love to not have this as a blocker".

## Technicalities of the career

What is the appropriate place for Jupyter Notebooks in the DS workflow?
- _[V]_ As you gain experience, you begin to think of tools as not necessarily good or bad. Just as good for X. Notebooks are good for the initial phases, not necessarily for production.

What should Data Scientists know about Software Engineering?
- _[A]_ Clean Code, Writing tests.
- _[E]_ Sometimes the constraints are different. E.g. For a one-off analysis, it might not need rigorous testing. Knowing how far to go can be good.

How much should Data Scientists should know about putting things into production?
- _[V]_ The more you learn the more "soft power" / flexibility you get.
- _[A]_ Knowing the end-to-end process can help. It can prevent you from getting blocked. Can learn from other DevOps people when possible.

How much should you master Cloud Technologies?
- _[V]_ Will eventually run into it on the job.
- _[A]_ Again, good to know to not get blocked.

Foundational Skills
- _[E]_ Python, R, Git/Github

Python vs R
- _[A]_ R for more Analyst jobs/work. Python end-to-end
- _[E]_ Seems like they are converging. R better for visualizations (ggplot), dplyr, shiny is good, and R usually has more cutting edge statistical stuff. (For a Python alternative to dplyr, see [Siuba](https://github.com/machow/siuba))
- _[A]_ Also, R better for Time Series

Can you make do with Python?
- _[A]_ For up to mid-sized companies, mostly yes.

Other technical stuff
- _[A]_ Knowing C, C++ can be helpful. Especially when speed-ups are required. Not necessary but being familiar with them can be a plus.
- _[V]_ Python, Unix, Json, yaml, and also a second language (Java, Go) to spot patterns across languages.

What technology are you learning ?
- _[A]_ Kubeflow, MLFlow, Sagemaker
- _[V]_ [Streamlit](https://github.com/streamlit/streamlit)
    - "The faster you can show your model, the better".
- _[E]_ Docker

## Data Science: Going forward

Will AutoML replace Data Scientists?
- _[A]_ ML Tools have become easier to use. But things like framing the business problem as ML problem will still require Data Scientists.

How will Data Science look in 3 years?
- _[V]_ Lot more consolidation. More platforms. And thus more work related to those kind of stuff. E.g. Connecting Sagemaker to Data Sources and a Dashboard.
- _[V]_ With the regulations that have been introduced, lot of companies are being and will be more cautious about what data they use.
- _[A]_ Companies hired a lot of Data Scientists, seeing them as an investment. This will probably decrease. They will be more selective, which is also good as it means they know who they want.

## Closing Remarks
- _[V]_ The job market is tough right now. Need to stand out. Learn Software Engineering, analysis. Have one project you can talk all the way through. Network around the community.
- _[A]_ Focus on the problem. Not the solution. Share what you do.
- _[E]_ Don't view what you find in the job market as an indication of your personal worth. Perhaps be more flexible now.

## Thoughts

The panelist had very sensible advice and insights. Personally, the part that interested me were the commentaries on the Data Science field, its evolution.
Also the practical aspects: how the jobs are in large part also about the person-role fit, possible ways to handle takehome exercises, and 
the helpful tip that a big differentiator in job applications is having someone inside who can vouch for you.

All in all, was fun listening in.
