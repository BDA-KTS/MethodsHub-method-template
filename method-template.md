# Methods Hub Method Template

The methods Hub method template is built using [cookiecutter.io](https://www.cookiecutter.io/). It helps to preload the project directory with the necessary files required for the Methods Hub i.e., 

- *postBuild* file to generate the method homepage and deploy the method in the interactive environment
- *README.md* with the desired subsections and their specifications
- Within project directory structure having
  - *Data* for the input and output files
  - *binder* for the postBuild and environment preserving files
  - *.github* for the GitHub workflows
- *CITATION.CFF* file for attribution
- Environment preservation files (*environment.yml* and *requirements.txt*)
- GitHub workflow file *methodshub.yml* to review the method 

## How to Use

- Execute ```cookiecutter``` to check if cookiecutter is installed
- If not
  - Execute ```python3 -m pip install --user cookiecutter``` or
  - Execute ```conda install cookiecutter```
- Execute the git clone path with the cookiecutter ```cookiecutter https://github.com/BDA-KTS/MethodsHub-method-template.git```. It internally uses git clone to clone the template repository locally while replacing the variables with the specific values for your project.
  - You will be asked for some variables to provide after the command e.g.., *project_slug*, *author_fîrstname*, *author_lastname*, and *author_orcid*
  - Some variables will be computed automatically e.g., *date*

These steps will deploy the method structure to write code, modify README.md and preserve the virtual environment.
