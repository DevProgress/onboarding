This will eventually have more information for both contributing to this project as well as what projects are acceptable for inclusion under DevProgress.

At the very least, all contributors must have a Contributor License Agreement.
If not, please sign up [here](http://devprogress.us/#joindp).

When starting a new repository:

1) Please copy "gitignore_template" to ".gitignore" (the leading "." is important) at the root level of your repository. [Git ignore documentation](https://git-scm.com/docs/gitignore). Then execute:

    git add .gitignore; git commit -m"gitignore"

in your shell.

2) Please only put "secrets" (passwords, API keys and such) in a file named "secrets.txt" at the root level of your repository AFTER you have created the gitingore file. This will prevent you from publishing DevPorgress passwords to the entire world.