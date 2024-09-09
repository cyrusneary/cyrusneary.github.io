---
permalink: /
title: "About me"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Welcome! I'm a postdoctoral researcher in the the [Robotics and Embodied AI Lab](https://montrealrobotics.ca/) at [Mila](https://mila.quebec/en) and [l'Université de Montréal](https://diro.umontreal.ca/accueil/). In Fall 2025, I will begin as an assistant professor in the Department of Electrical and Computer Engineering at [The University of British Columbia](https://ece.ubc.ca/).

I received a Ph.D. in Computational Science, Engineering, and Mathematics from [The Oden Institute](https://www.oden.utexas.edu/) at The University of Texas at Austin in 2024. There, I worked with Professor Ufuk Topcu as a member of the [Center for Autonomy](https://oden.utexas.edu/research/centers-and-groups/center-for-autonomy/). I was also a member of the [Center for Scientific Machine Learning](https://oden.utexas.edu/research/centers-and-groups/center-for-scientific-machine-learning/). 
<!-- I'm a member of Professor Ufuk Topcu's [Autonomous Systems Group](https://www.ae.utexas.edu/facultysites/topcu/wiki/index.php/Main_Page).  -->

Prior to my graduate studies in Austin, I obtained a Bachelors of Applied Science degree from The University of British Columbia, where I studied Engineering Physics and minored in Honours Mathematics.

### Research Interests
Realizing the full potential of artificial intelligence (AI) requires a dual approach: developing engineering methodologies to design AI systems, and designing AI algorithms to solve specific engineering problems. My research leverages this dual perspective to develop AI systems for purposes of **control, robotics, autonomy, dynamics modeling, and computational engineering**. Specifically, my research asks: how can we engineer AI systems within budget constraints, certify them against stakeholder requirements, and ensure that they meet the needs of the end user? On the other hand, how can we design AI algorithms that embrace the unique characteristics of engineering applications?

Towards answering these questions, my research develops theory and algorithms that span topics from **multiagent reinforcement learning, to physics-informed machine learning, to the reliable use of large language models in the design of autonomous systems**. More broadly, my research addresses the diverse and ever-expanding challenges and opportunities associated with engineering AI systems to tackle societally impactful problems. 
<!-- I have applied these algorithms to enable unprecedented autonomy for air and ground robots; I developed a multifidelity simulation-to-reality pipeline to train, verify, and deploy deep reinforcement learning policies that pilot unmanned ground vehicles, and I used physics-informed learning to develop model-based controllers for hexacopter hardware from extremely scarce datasets. -->

If you're interested in learning more, click [here](publications.md) for a list of my recent projects.

<!-- I'm interested in studying how prior knowledge can be incorporated into deep learning and reinforcement learning algorithms in order to improve their data efficiency and their generalizability, as well as to yield policies with verifiable properties. Two of my recent projects have focused on [compositional RL systems](../_publications/2021_verifiable_and_compositional_rl.md), and on [using physics-based knowledge](../_publications/2023_how_to_sde_in_3_mins.md) to improve the data efficiency and generalizability of neural network models of dynamical systems. -->

<!-- Developing methods to incorporate prior knowledge into reinforcement learning algorithms in order to improve their data efficiency and robustness, as well as to yield policies with verifiable properties. -->


<!-- I'm interested in studying how prior knowledge can be incorporated into reinforcement learning systems, and how such structured information may be used for the formal verification of said systems. -->

<!-- He is interested in studying how prior knowledge can be incorporated into reinforcement learning (RL) systems, and how such information may be used for the formal verification of said systems, particularly in the context of safety-critical engineering applications. His recent research has focused on compositional RL systems; complex (or multi-agent) systems are decomposed into their constituent components to simplify learning, while theoretical guarantees are developed to assure that compositions of such components satisfy system-level requirements. -->

<!-- **Other Intersts**
In my free time I enjoy reading fiction, taking photos, and playing video games. -->

<!-- This is the front page of a website that is powered by the [academicpages template](https://github.com/academicpages/academicpages.github.io) and hosted on GitHub pages. [GitHub pages](https://pages.github.com) is a free service in which websites are built and hosted from code and data stored in a GitHub repository, automatically updating when a new commit is made to the respository. This template was forked from the [Minimal Mistakes Jekyll Theme](https://mmistakes.github.io/minimal-mistakes/) created by Michael Rose, and then extended to support the kinds of content that academics have: publications, talks, teaching, a portfolio, blog posts, and a dynamically-generated CV. You can fork [this repository](https://github.com/academicpages/academicpages.github.io) right now, modify the configuration and markdown files, add your own PDFs and other content, and have your own site for free, with no ads! An older version of this template powers my own personal website at [stuartgeiger.com](http://stuartgeiger.com), which uses [this Github repository](https://github.com/staeiou/staeiou.github.io).

A data-driven personal website
======
Like many other Jekyll-based GitHub Pages templates, academicpages makes you separate the website's content from its form. The content & metadata of your website are in structured markdown files, while various other files constitute the theme, specifying how to transform that content & metadata into HTML pages. You keep these various markdown (.md), YAML (.yml), HTML, and CSS files in a public GitHub repository. Each time you commit and push an update to the repository, the [GitHub pages](https://pages.github.com/) service creates static HTML pages based on these files, which are hosted on GitHub's servers free of charge.

Many of the features of dynamic content management systems (like Wordpress) can be achieved in this fashion, using a fraction of the computational resources and with far less vulnerability to hacking and DDoSing. You can also modify the theme to your heart's content without touching the content of your site. If you get to a point where you've broken something in Jekyll/HTML/CSS beyond repair, your markdown files describing your talks, publications, etc. are safe. You can rollback the changes or even delete the repository and start over -- just be sure to save the markdown files! Finally, you can also write scripts that process the structured data on the site, such as [this one](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb) that analyzes metadata in pages about talks to display [a map of every location you've given a talk](https://academicpages.github.io/talkmap.html).

Getting started
======
1. Register a GitHub account if you don't have one and confirm your e-mail (required!)
1. Fork [this repository](https://github.com/academicpages/academicpages.github.io) by clicking the "fork" button in the top right. 
1. Go to the repository's settings (rightmost item in the tabs that start with "Code", should be below "Unwatch"). Rename the repository "[your GitHub username].github.io", which will also be your website's URL.
1. Set site-wide configuration and create content & metadata (see below -- also see [this set of diffs](http://archive.is/3TPas) showing what files were changed to set up [an example site](https://getorg-testacct.github.io) for a user with the username "getorg-testacct")
1. Upload any files (like PDFs, .zip files, etc.) to the files/ directory. They will appear at https://[your GitHub username].github.io/files/example.pdf.  
1. Check status by going to the repository settings, in the "GitHub pages" section

Site-wide configuration
------
The main configuration file for the site is in the base directory in [_config.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_config.yml), which defines the content in the sidebars and other site-wide features. You will need to replace the default variables with ones about yourself and your site's github repository. The configuration file for the top menu is in [_data/navigation.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_data/navigation.yml). For example, if you don't have a portfolio or blog posts, you can remove those items from that navigation.yml file to remove them from the header. 

Create content & metadata
------
For site content, there is one markdown file for each type of content, which are stored in directories like _publications, _talks, _posts, _teaching, or _pages. For example, each talk is a markdown file in the [_talks directory](https://github.com/academicpages/academicpages.github.io/tree/master/_talks). At the top of each markdown file is structured data in YAML about the talk, which the theme will parse to do lots of cool stuff. The same structured data about a talk is used to generate the list of talks on the [Talks page](https://academicpages.github.io/talks), each [individual page](https://academicpages.github.io/talks/2012-03-01-talk-1) for specific talks, the talks section for the [CV page](https://academicpages.github.io/cv), and the [map of places you've given a talk](https://academicpages.github.io/talkmap.html) (if you run this [python file](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.py) or [Jupyter notebook](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb), which creates the HTML for the map based on the contents of the _talks directory).

**Markdown generator**

I have also created [a set of Jupyter notebooks](https://github.com/academicpages/academicpages.github.io/tree/master/markdown_generator
) that converts a CSV containing structured data about talks or presentations into individual markdown files that will be properly formatted for the academicpages template. The sample CSVs in that directory are the ones I used to create my own personal website at stuartgeiger.com. My usual workflow is that I keep a spreadsheet of my publications and talks, then run the code in these notebooks to generate the markdown files, then commit and push them to the GitHub repository.

How to edit your site's GitHub repository
------
Many people use a git client to create files on their local computer and then push them to GitHub's servers. If you are not familiar with git, you can directly edit these configuration and markdown files directly in the github.com interface. Navigate to a file (like [this one](https://github.com/academicpages/academicpages.github.io/blob/master/_talks/2012-03-01-talk-1.md) and click the pencil icon in the top right of the content preview (to the right of the "Raw | Blame | History" buttons). You can delete a file by clicking the trashcan icon to the right of the pencil icon. You can also create new files or upload files by navigating to a directory and clicking the "Create new file" or "Upload files" buttons. 

Example: editing a markdown file for a talk
![Editing a markdown file for a talk](/images/editing-talk.png)

For more info
------
More info about configuring academicpages can be found in [the guide](https://academicpages.github.io/markdown/). The [guides for the Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/configuration/) (which this theme was forked from) might also be helpful. -->
