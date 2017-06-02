# Mozilla Mini Grant application

***1st June 2017***

### Applicant Details

**Name:** Isla Staden

**Email:** istaden@turing.ac.uk

**Physical address:**

Alan Turing Institute<br>
British Library<br>
96 Euston Road<br>
London NW1 2DB

**Institution:** Alan Turing Institute

**Have you previously received a grant from the Mozilla Foundation?**
*If so, list the amount and purpose of the grant.*

No.

### Proposal summary

**Title** *(10 words)*: Brain Networks in Python

**Provide a brief description of your project or event**

*(50 words)*

The Brain Networks in Python project provides open source, documented, tested and modular code to investigate the brain as a network. These analyses are reproducible, transparent and accessible to new and expert brain imaging researchers and network neuroscientists. Openly developed, this project welcomes users and contributors from all disciplines.

**Total proposal budget in US Dollars (USD)**:

4,960

**How much money in USD are you requesting from the Mozilla Foundation?**

4,960

**List your partners, if any, and the role/s they will play.** *(250 words)*

I will be mentored by Dr Kirstie Whitaker. Kirstie is a research fellow at the Turing Institute and outgoing Mozilla Fellow for Science. She is a neuroscientist who studies brain development, using graph theory to understand the brain as a network. Dr Whitaker is a two time mentor for the Mozilla Open Leadership Training Series and she has extensive skills in nurturing and supporting open projects. The Brain Networks in Python is built within the Whitaker Lab GitHub repository where Dr Whitaker is an active contributor. She will review all code and documentation and provide guidance to ensure the Brain Networks In Python project is accessible and usable for all.

I will also work with the research software engineering team at the Alan Turing Institute. The team is lead by Dr James Heatherington who has worked for 5 years as the head of Research Software Development at University College London. In his words: "Well written, readable software, written for humans to read as well as computers to execute, forms an important part of research communications and can deliver significant research impact." ([http://www.ucl.ac.uk/research-it-services/people/james](http://www.ucl.ac.uk/research-it-services/people/james))

**On which Internet health issue(s) does your proposal focus?**

- [x] Open Innovation
- [ ] Digital Inclusion
- [ ] Decentralization
- [ ] Privacy and Security
- [ ] Web Literacy

**If you are NOT a US resident or citizen will the proposed project or event involve travel to or activities within the United States?**

- [ ] Yes
- [x] No
- [ ] Not applicable

**Are you requesting support for an event or a project?**

- [ ] Event
- [x] Project

### Proposal description

**Describe the issue/problem you are trying to address.** *(100 words)*

The brain made up of many regions that communicate millions of messages every second. Traditional neuroimaging analyses have considered each region separately and therefore failed to capture many aspects of brain structure and function. Graph theory allows us to analyse human brain images as a network ([Bullmore & Sporns, 2009]()). The most popular toolbox to do brain network analyses is written in Matlab (Brain Connectivity Toolbox: https://sites.google.com/site/bctnet) which requires an expensive (and therefore inaccessible) license. We want to provide free and openly available software to allow all neuroscience researchers to conduct reproducible and biologically meaningful investigations of the human brain.


**List key project activities (what you will do), outputs (what will be produced through your activities) and outcomes (impact of your project on your beneficiaries during the grant period).** *(1000 words)*

*Activities*

The Brain Networks in Python code was implemented in the Neuroscience in Psychiatry Network publication "Adolescence is associated with genomically patterned consolidation of the hubs of the human brain connectome" published in PNAS in 2016 ([Whitaker\*, Vertes\* et al, 2016](http://dx.doi.org/10.1073/pnas.1601745113)). The code conducts structural covariance network analyses on cortical thickness measurements from two independent cohorts and creates all figures and results tables for the published manuscript. The code and data to support the manuscript can be found at [https://github.com/KirstieJane/NSPN_WhitakerVertes_PNAS2016](https://github.com/KirstieJane/NSPN_WhitakerVertes_PNAS2016).

As currently written, the Brain Networks in Python code is monolithic. It is very difficult to repurpose for new analyses or for different datasets. The first goal of this project will be to *refactor the code into modules*. Specifically, I will break down the conceptual steps for a network analysis and allow the user to re-combine them as they see fit. For example, one user may want to use the code only for the graph theory measures while another may use the visualisation module alone. It will be possible to link the modules together to complete an entire neuroimaging analysis from start to finish, but this workflow will not be necessary. Modularising the software will permit a more diverse user base and a much more interoperable set of code.

The second best time to add in tests for software is when refactoring. (The optimum time would have been when the code was written in the first place). As part of this 2 month project we will *add in high level and unit tests* for the network analysis code. Testing will give users confidence in our code and allow us to implement continuous integration. We are already developing in a version controlled enviroment on GitHub, but as the project develops, we will always be able to verify the accuracy of the modules.

We will also add *new functionality* to the code. There is currently no way (in this codebase) to investigate the difference in brain networks between two groups. For example, a key question in the field of biological psychiatry is whether the brains of people who have a diagnosis of depression are differently connected to the brains of healthy control participants. We will add a module that permutes the original data and builds up a null distribution so that differences between the two real groups, for example people with a diagnosis of depression and healthy controls, can be statistically tested.

Along with integrated tests, *documentation* will allow the Brain Networks in Python code to be used by many people. We will provide example data and clear tutorials to make it easy for users to install and get up and running with the code. These tutorials will be in the form of Jupyter notebooks that can be either downloaded and run locally or run in a MyBinder ([http://mybinder.org](http://mybinder.org)) instance online. An example Jupyter notebook that is currently in development can be found at [https://github.com/WhitakerLab/BrainNetworksInPython/blob/master/Example_JupyterNotebook.ipynb](https://github.com/WhitakerLab/BrainNetworksInPython/blob/master/Example_JupyterNotebook.ipynb).

Finally, we will release our code as a python packages that can be easily installed via pip (https://packaging.python.org) or conda (https://conda.io). We will ensure that all released versions of our code have digital object identifiers from Zenodo ([https://zenodo.org](https://zenodo.org/)).

*Outputs*

* MIT licensed, documented and tested code that is easy to use and re-use.
* Modular code that can be repurposed for individual use cases.
* An easy to install and version controlled python package that can be cited in future publications.
* Version controlled code that permits rigorous reproducible neuroscience.
* An open and inclusive community dedicated to supporting new and veteran users and contributors.

Once a community grows around the project we hope to inspire additional integrations. For example collaborating with Mozilla Global Sprint project Cytoscape js ([http://js.cytoscape.org](http://js.cytoscape.org/)) to provide interactive visualisations of the networks. We could also harness the power of Docker containers promoted by BIDS (Brain Imaging Data Structure) Apps ([http://bids-apps.neuroimaging.io](http://bids-apps.neuroimaging.io/)) to make it even easier for analyses to be reproducible and accessible.

*Outcomes*

Make it easier to replicate analyses. Make network analyses more accessible.

Smoother onboarding. Ensure early career researchers can conduct cutting edge neuroimaging analysis in a documented and community supported enviroment.

Better science. Better understanding of the brain!

Lots of exciting extensions. Interactive visualisation, extension to different types of networks.

**Provide key indicators you plan to use to measure project outcomes and source of data.** *(500 words)*

DOI

> All projects should specifically reflect priorities that enhance our broader community efforts toward open innovation, efficiency in regards to practicing open science (lower barriers, ease of use & integration, etc), and reproducibility (transparent research methods & results).

Gooooooood question. I'm not sure. Probably the best would be some papers to come out of it!

* Simone?
* Paula?
* Kirstie NORA

**Explain who will benefit from the project.** *(100 words)*

AAAAAALSO A good question. Scientists. People wanting to study brain as a complex network. Network analysists who want to apply their methods to brain networks? <-- good idea, could be that there are people with graph theory specific knowledge who have ideas about how you should analyse the brain. The open source code would allow them to see and improve our analysis

Allows provenance of analysis and efficient knowledge transfer, so this project also benefits senior scientists who are mentoring members of their group. They don't have to be concerned about

**List any risks or challenges that may affect the overall success of your project and now how Mozilla and/or others can help you to overcome these challenges.** *(250 words)*

These are ALL VERY GOOD POINTS.

Probably the biggest challenge is that it is not usable for others - currently code works perfectly for the Neuroscience in Psychiatry Network but requires Kirstie's idiosyncratic knowledge! Best way forward is to link into the Mozilla network and get early feedback from the community.

**Is this a new project or continuation? If new, please describe your qualifications to initiate the activity. If continued, please describe your accomplishments to date. Feel free to include links to articles and documents online that highlight your recent work.** *(1000 words)*

Continuation of Kirstie's work. INSERT DESCRIPTION OF PNAS PAPER.

New for Isla. INSERT expertise re: graph theory & networks etc.

* Degree in Maths from Cambridge - including graph theory course.
* Advanced coding in Python - matplotlib, networkx, numpy, pandas - git & GitHub, LaTeX and matlab.
* Already working on the code - jupyter notebook


**Mozilla works in the open. How will you document and share your project progress with the community.** *(250 words)*

GitHuuuuuuub. Already there. Twitter account for lab.

Got a contributing file and code of conduct. Building issues during mozilla global sprint and updating README file.

Embrace working open philosophy. Ensure that work in progress is shared so that others can provide help and feedback.

IS:

* We work so openly that our weekly meetings notes are public.
* It's fun for me to keep writing blog articles about our progress


**How will you continue work on this project beyond the funding period?** *(250 words)*

We hope that users will continue to contribute. Kirstie will be able to monitor contributions.

Isla....applying for other funding? Planning to apply for masters programs in maths - network analyses will support these endeveavors.

Importantly - doesn't need to be "me". Whole point of building documentation openly is so that others can fork and contribute even if Isla leaves!

### Upload documents

**Please upload an itemized project budget using the template linked below.**

[http://bit.ly/2riERqd](http://bit.ly/2riERqd)

### Communications

**How did you hear about the mini-grant opportunity?**

- [x] Twitter
- [x] Blog
- [ ] Friend
- [ ] Other

**Do you want to be added to our Mozilla Science Lab mailing list?**

- [x] Yes
- [ ] Not at this time

---

Kirstie's Brain Networks In Python code is already available on github, we want to expand the code base, add tests and improve usability by creating detailed documentation and providing step by step instructions. In short, we want to make the code open source in a greater sense than just putting it out there.
This will serve two purposes. The first: anyone will be be able to learn from it and use it to run network analyses on their own data with minimal friction. It will be straight forward for users to add their own features an build on the code base as needed. The second purpose addresses reproducibility in science. When someone (Kirstie or anybody else) reports a finding using these tools and makes their data available, everything can be checked. We allow people to check the results by providing clear instruction for beginners users- and to check the methodology, by making our code transparent, well-documented and testable.

The goal Kirstie and I have is to show how easy it is to take something you have written for your own analysis purposes and make it useful to others and, by making your analysis reproducible, useful to yourself.