# Part 3 - Create your own science project!

Part three is about creating and hosting your science project on Github.

## Tasks

* Think of a short and precise (and cool) name for your project.
* Create your own repository using our [science project template](https://github.com/climate-service-center/science-project)
  * Click on ![grafik](https://github.com/user-attachments/assets/d96dd066-d70a-4b98-aff3-1def1e42df8e).
  * In the field for "Repository name" enter the name of your project.
  * wait until the repository is created in your personal profile.
* Rename the folder `science_project` to the name of your own project.
* In the file `pyproject.toml`, rename the project name and setuptools packages entry according to your project.
  * Update the `name = "science-project"`.
  * The `packages` entry has to be the name of the subfolder you should have already renamed.
* Clone the package to your computer and install it in a new environment in [editable mode](https://setuptools.pypa.io/en/latest/userguide/development_mode.html):
  * In your package directory (where the `pyproject.toml` file lies), try `pip install -e .`
  * This will also install all requirements you define in the `requirements.txt` file! Check it out!
