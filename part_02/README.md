# Part 2 - Working together

Everybody should be setup and comfortable with creating their own repositories on github and/or gitlab and make commits. In part 2, we want to actually work together
on a repository. If you want to know more details, please check:

* [Collaborating with pull requests](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests) (github)
* [Merge requests](https://docs.gitlab.com/ee/user/project/merge_requests) (gitlab)
* [Interactive course: Introduction to github](https://github.com/skills/introduction-to-github)

For this part, we created a demo repository on which we want to work together. Depending on what you prefer, there is one on [github](https://github.com/climate-service-center/say-your-name) and one in [gitlab](https://codebase.helmholtz.cloud/gerics_infrastructure/say-your-name).

## Tasks

* [Fork](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo#forking-a-repository) the demo repository (here is the one on [github](https://github.com/climate-service-center/say-your-name) and here in [gitlab](https://codebase.helmholtz.cloud/gerics_infrastructure/say-your-name)) for this tutorial to your personal github account or [create a fork in gitlab](https://docs.gitlab.com/ee/user/project/repository/forking_workflow.html#create-a-fork) respectively.
* [Clone the fork](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo#cloning-your-forked-repository) to your local computer.
* Create and checkout a new branch using `git checkout -b my-name`.
* Check using `git status`.
* Add a feature, e.g., copy the existing `lars.py` to a new file with your name (Don't forget to also adapt the source code!). Make it say your name!
* Check using `git status`. What does it say?
* Add your new file using `git add` and `git commit`.
* Push the changes from your branch to a remote branch in your fork using `git push origin my-name`.
* [Create a pull request from your fork](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork) on github and write a nice message to the maintainers or create a [merge request in gitlab](https://docs.gitlab.com/ee/user/project/merge_requests/creating_merge_requests.html).
* When the pull request was accepted, [sync your fork](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/syncing-a-fork#syncing-a-fork-branch-from-the-web-ui)! Here is [how to do it in gitlab](https://docs.gitlab.com/ee/user/project/repository/forking_workflow.html#update-your-fork).
