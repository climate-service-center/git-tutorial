<img src="https://mirrors.creativecommons.org/presskit/logos/cc.logo.large.png" width="150" align="right"/>

# Git tutorial

**Collaborate, communicate and publish code using git and github/gitlab.**

This should be a very basic guide on how to publish your codes, software and data to make it available to a broader public or just your colleagues next door. It's more or less a compilation of existing resources on this topic. Note that this guide does not claim to be finished, the whole truth or perfect at all. If you have experience with writing scientific codes, you might find this guide incomplete. If you usually write code only for your own without sharing it, you might be overwhelmed. However, to cover some common ground, we want to raise awareness and focus your attention on your code being an integral part of your scientific work and publication.

## Motivation

Most of our publications and products are based on data processing and analysis. Good scientific practice also includes [**reproducibility and reusability**](https://gfzpublic.gfz-potsdam.de/pubman/faces/ViewItemOverviewPage.jsp?itemId=item_5005567) of codes and data as key and they are central concerns of the [Helmholtz Open Science Initiative](https://os.helmholtz.de/). In fact, making your research codes and data tidy, reproducible and reusable is nowadays much easier and fun than most scientists think and it can considerably improve your ability to cooperate with your peers and colleagues. It should be more a kind of attitude towards working transparently than simply a tedious task.

![grafik](https://github.com/climate-service-center/git-tutorial/assets/5659125/1209b650-0a33-4741-af97-737a0ddc391f)

## Preparation

To preare for the tutorial, you should check if you have git installed and can use it in a terminal. If you have no git installation, you can follow the instructions of the [official documentation](https://git-scm.com/downloads). You will also need to use a platform for sharing your code, e.g., make sure you have a github account you can access or use your gitlab account at the [Helmholtz codebase](https://codebase.helmholtz.cloud/). For the Helmholtz codebase, you can use any Helmholtz account to login via the [Helmholtz AAI](https://hifis.net/aai). You will also need to be able to *push* to github/gitlab for which you have to create and register an ssh key with github/gitlab. For this, use and existing or create a new ssh key on your local computer and store the public key, e.g., in [your github profile settings](https://github.com/settings/keys) and/or your [gitlab account](https://docs.gitlab.com/ee/user/ssh.html#add-an-ssh-key-to-your-gitlab-account). For more detailed instructions, please also follow, e.g., the [official github documentation](https://docs.github.com/en/authentication/connecting-to-github-with-ssh).

If you are a Windows user with no experience in git or using the terminal, we recommend the following based on own experience:

### how to setup git on windows

* Install git on your windows machine (if is not installed already). You may invoke in your Windows Power Shell the following command (assuming your default location is U:
  ```bash
  U:\> winget install --id Git.Git -e --source winget
  ```
  This should install all software of the [git for Windows](https://gitforwindows.org/) tool set.
* Open "git GUI" and go to the menu "Help/show SSH key"
* If not key is found, then click on "Generate key" to generate a new ssh key. If you get an error concerning missing `.ssh` folders, you might have to create that yourself, e.g., `mkdir .ssh`.
* Copy the content of the public ssh key.
* Go to Github in your web browser and in the settings menu go to [SSH and GPG keys section](https://github.com/settings/keys). Click on "New ssh key" and paste your public ssh key.
* Open a "git bash" terminal and test your git connection by invoking the following command:
  ```bash
  ssh -T git@github.com
  ```
  
## Planning

The publication of code and data should receive the same focus of attention and planning as a *classical* scientific paper publication. It should be an important part when you [plan a project](https://the-turing-way.netlify.app/project-design/project-design.html). The best thing to do is to always start writing your code having this in mind and ask yourself honestly: 

* Will somebody else be able to understand what i did? 
* Will he/she be able to run my code and reproduce my results/plots (without complicated explanations)?
* How can i make life easier for them?

If you have these things in mind during writing your code, you are already on a good way. 

Luckily, there are some very helpful tools and methods to help you getting your code organized. The Helmholtz Open Science Seminar has presented some very [helpful guidance](https://gfzpublic.gfz-potsdam.de/pubman/item/item_5005567) and a [factsheet](https://doi.org/10.48440/os.helmholtz.025) to help researchers getting their code on track for easier collaboration, reproducibility and fun! Here is an excerpt from the factsheet

![grafik](https://github.com/climate-service-center/git-tutorial/assets/5659125/bbb5cff6-87e2-48cb-b184-bbe8be978b25)

## Start with a project repository

Even when you have not written any code yet, you should start your project by [creating a project repository](https://the-turing-way.netlify.app/project-design/project-repo.html), e.g., on [github](https://docs.github.com/en/get-started/using-git/about-git) or the [Helmholtz codebase](https://gitlab.hzdr.de/). This can be a great landing page for your project. If you start by writing a comprehensive `README.md`, you can simply refer colleagues and collaborators to your project page where they can find all neccessary information without you having to explain it all over again. You can also structure your project more efficiently by using the repositories isse mangaement. You can also check out the [github](https://docs.github.com/en/pages/quickstart)/[gitlab](https://gitlab.com/pages) pages feature which will enable you to create nice webpages easily from your project repository.

## Checklist for publication

If you publish your code, you should be aware of some basic technical requirements that should be checked. If you have followed some of the advice above, you should easily be ready to publish. However, the minimum requirements are:

* A publically accessible project repository.
* A `README`, preferrably in markdown format that should include some information on your project, further links and basic technical documentation.
* [License](https://www.astrobetter.com/blog/2014/03/10/the-whys-and-hows-of-licensing-scientific-code/) (check if you have used GPL licensed libraries!)
* `environment.yml` or `requirements.txt` file that defines software dependecies.
* DOI, e.g., using [`zenodo`](https://zenodo.org/), works well with [github](https://docs.github.com/en/repositories/archiving-a-github-repository/referencing-and-citing-content).

You can use [howfairis](https://github.com/fair-software/howfairis) to automatically check some basic requirements of FAIR principles for your project repository.

## Examples

Here is a short list of publications by GERICS employees which might be good examples for code and data publication:

* [Principles](https://github.com/KatharinaBuelow/cmip5_cmip6_euro-cordex-plotting-routines)
* [LEAFlood](https://github.com/TWuebbelmann/LEAFlood)
* [Wind stilling](https://github.com/jwohland/stilling_MPI-GE)
* [Irrigation analysis](https://github.com/ChristinaAsmus/irrigation_param_analysis)
* [pyremo](https://github.com/remo-rcm/pyremo)

## Further fun reading

* [The Turing Way Handbook](https://the-turing-way.netlify.app)
* [Does your code stand up to scrutiny?](https://doi.org/10.1038/d41586-018-02741-4)
* [Nature Checklist](http://www.nature.com/documents/GuidelinesCodePublication.pdf)
* [AGU Data and Software Guide](https://www.agu.org/Publish-with-AGU/Publish/Author-Resources/Data-and-Software-for-Authors)
* [Open up to Open Science](https://issues.org/opening-up-open-science-gentemann-erdmann-kroeger/)
* [Scientific collaboration and project management in github](https://rabernat.medium.com/scientific-collaboration-and-project-management-in-github-d74f2255ae5f)
* Barnes, N. Publish your computer code: it is good enough. Nature 467, 753 (2010). https://doi.org/10.1038/467753a
* [UNESCO recommendations on open science](https://unesdoc.unesco.org/ark:/48223/pf0000379949.locale=en)
