# git-tutorial
git and github tutorial

## preparation

### how to setup git on windows
1. Install git on your windows machine (if is not installed already).
  You may invoke in your Windows Power Shell the following command
  (assuming your default location is U: :

  PS U:\> winget install --id Git.Git -e --source winget

2. Open "git GUI" and go to the menu "Help/show SSH key"
3. If not key is found, then clic on "Generyte key" to generate a new ssh key.
4. Copy the content of the public ssh key just recently created.
5. Go to Github in your web browser and in the settings menu go to "SSH and GPG keys" section. Clic on "New ssh key" and paste your public ssh key.
6. Open a "git bash" and test your git connection by invoking the following command:
   
   $ ssh -T git@github.com
