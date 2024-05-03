# git-tutorial

Collaborate, communicate and publish on github.

## preparation

To preare for the tutorial, you should check if you have git installed and can use it in a terminal. If you have no git installation, you can follow
the instructions of the [official documentation](https://git-scm.com/downloads). If you want to push to github (or a gitlab instance), you have to create and register an ssh key with github/gitlab.
For this, use and existing or create a new ssh key on your local computer and store the public key, e.g., in [your github profile settings](https://github.com/settings/keys). For more detailed instructions,
please also follow, e.g., the [official github documentation](https://docs.github.com/en/authentication/connecting-to-github-with-ssh).

If you are a Windows user with no experience in git or using the terminal, we recommend the following based on own experience:

### how to setup git on windows

* Install git on your windows machine (if is not installed already). You may invoke in your Windows Power Shell the following command (assuming your default location is U:
  ```bash
  U:\> winget install --id Git.Git -e --source winget
  ```
  This should install all software of the [git for Windows](https://gitforwindows.org/) tool set.
* Open "git GUI" and go to the menu "Help/show SSH key"
* If not key is found, then clic on "Generyte key" to generate a new ssh key.
* Copy the content of the public ssh key just recently created.
* Go to Github in your web browser and in the settings menu go to "SSH and GPG keys" section. Clic on "New ssh key" and paste your public ssh key.
* Open a "git bash" and test your git connection by invoking the following command:
  ```bash
  ssh -T git@github.com
  ```
