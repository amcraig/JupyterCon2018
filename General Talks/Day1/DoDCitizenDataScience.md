# Citizen data science: An enterprise use case from inside the US intelligence community

Dave Stuart: Department of Defense

>Jupyter in the enterprise level 
>Challenges at scale

Typical workflow for a DoD analyst is meanial manual tasks to access and modify data, ultimately to export to do final analysis on Excel

Also empowering Analysts to write reproducible workflow

Instead of thinking in terms of tools, their thought process switched to thinking in terms of questions and answer

>"While expecting some analysts to write/read code is reasonable, expecting them to be sysadmins is not"

Tens of thousands of enterprise users, hired for their domain experience, were not hired for coding potential

Large geographically diverse userbase

Huge data security Challenges
* Sensitive subject matter
* extermely finegrained security
* Input data varies by time and user

Complience Challenges

They supply a prebuilt Jupyter environment personalized VMs, easily spun up, all configured the same, Ephemeral - self destructible 

## nbgallery 
* nbgallery sharing and collaboration platform (code only - DoD)
* Open source released
* Easy to use repo of community authored notebooks

Only shows rendering of the code of the notebook need to export to Jupyter notebook in order to use

They also rank nbs on trendiness, helpfulness, recommendations, health of code (does it need work)

They also cluster them by your type of role (are you new)

## Broken notebooks break confidence in the community with them

Code health will decay over time

[White paper](https://nbgallery.github.io/health_paper.html)

Need to find a balence between training and a demanding workload. They're not expected to be a data scientist, just be able to look at code and use pre made cells

"Intro to Python for Analysis" - Class

People who run the notebooks may get different results based on classified information clearance, therefore everyone needs to modify their own notebooks for personal use cases

DoD is heavy users of ipywidgets

Jupyter provides trade/craft transparency

All the notebooks query APIs not paths or hard coded