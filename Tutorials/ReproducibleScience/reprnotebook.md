# Preparing your Jupyter Notebook for computationally reproducible publication:

[Link to the Slides](shorturl.at/abuwB)

## Computational reproducablility:
The complete software development environment and the complete set of instructions which generated the figures

Jupyter notebooks are great for documenting your methods

Are Jupyter Notebooks good enough to fully encapsulate methods?

Is it well documented, not misleading, does everyone get the same results? <br>
Can average people even figure out how to run it without running into problems?<br>
Are we assuming the end user is a Linux user?

* Link to your repositories
* Obtain a DOI
* Don't make assumptions on platforms
* Bundle dependancies rather than retrieve on demand
a* Perhaps, make a container with clear instructions on its execution

Four tenants of reproducability:
 * Organization
 * Documentation
 * Automation
 * Dissemination

(Try to write down dependencies ASAP after experiment)

## **Organize** 
* Archive the exact versions of data used and include them in your respository
* Bundle dependencies and include them in your repository rather than retrieve on demand
* Link to repositories rather than directly to rendered notebooks

A Code Ocean Capsule is a encapsulated AWS / Docker / Code Executor / Repository hub, but online for all to use - Platform agnostic (You could even change the setup script to a Windows environment *if you really wanted to*)

Cloudocean is a service devoted to to computational reproducibility

Organize your research to separate code + notebooks from data.

[Link to April's Repo for the Data](https://github.com/aprilcs/candy_trade)

## **Document** 
We can configure a container for your notebooks with Docker, binder, or Code Ocean.

You can freeze your dependencies in a requirements.txt

The Code Ocean capsule has a *env* tab that automatically documents **how** and **what** dependencies your code requires 

* Specify your packages and dependencies with versions.
    * pip freeze > ../code/requirements.txt
    * conda list --export > ../code/requirements.txt
    * i.e. pandas==0.13 #not an actual version number 

* Create a Data Dictionary
    * Is a separate md/txt file that lists the terms 
    * This could be redundant if you have such a robust notebook
    * There is no style guide for this yet
    * Elaborates on what the terms found in your data mean

## **Automate**
>Manual manipulation or setup was needed to reproduce results, often without documentation of how the results were produced. - Woodbridge et al.

We can automate the execution of our notebooks:
* Create a master script to execute all notebooks and analyses (can be anything you want: Python, Shell).
* Reproduce results automatically as a function of the data & the code; Save results explicitly.
* Use relative paths.

Try to develop notebooks that are **not interactive** for ease of automation

Output files are saved in sessions for differing 

## **Dissemination**
There is no standardized way of attaching notebooks to published articles.
Therefore it is difficult to discover and retrieve notebooks.

We can embed or link notebooks persistently:
* Obtain a DOI for your repository and use this link throughout your article.
    * Example: Github -> Binder -> Zenodo -> DOI linked in article
    * Example: CodeOcean -> DOI in article
* Cross link repository with published article in metadata of each.
* Embed executable capsule within the article.
    * Example: https://f1000research.com/articles/4-121/v1

Specify a license for your data and your code + notebooks.
Resources on choosing a data licence:

Digital Curation Center: http://www.dcc.ac.uk/resources/how-guides/license-research-data

Resources on choosing a code licence:
* Karl Broman: http://kbroman.org/steps2rr/pages/licenses.html

Open Source Initiative: https://opensource.org/licenses





