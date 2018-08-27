# Reproducible Quantum Chemistry in JupyterLab

Chris Harris: Kitware @openchem

[OpenChem](https://www.openchemistry.org/)
[Github](https://github.com/openchemistry)

>Explore a platform that uses Jupyter to enable reproducible quantum mechanics calculations in the browser, using a powerful data server coupled with cloud or high-performance computing resources on the server side

## Scientific Use Case

Computational Chemistry has a lack of transparent and reproducible workflows

Most Comp Chemistry simply don't have the skills for HPC

Need a platform for end-to-end support

## Why Jupyter

Supports interactive analysis while preserving the analytic steps

Linear structure is friendly for users

Familiar in the comp chem domain already

Great ecosystem and community

## Approach

* Data at the core
* RESTful API everywhere
    * Notebooks, Webapps, commandline ,desktop applications
* Jupyter notebook for interactive analysis 
* Web application with login from anywhere

Jobs take several minutes to run even for small systems

## Example

Post-Talk Realized that the example is on:
[example](https://github.com/OpenChemistry/openchemistrypy/blob/master/examples/openchemistry.ipynb)

```python
import openchemistry as oc
asprin = oc.somethingstructurefromname('Asprin')

ethanol = oc.findstructure('inchikeyforethanol')

calc setup = {
    vasis:'3-21g',
    'functional': 'B3LYP
}

result = ethanol.optimise(**calc_setup )
result.orbital.show()

result.orbitals.url() # can view model with ANY user

result = ethanol.frequencies(**calc_setup)
results.frequencies.show(mode = 56, animate_modes=true)

elements = [F,Cl,'Br']
template = a variable string that will input elements from list to generate three equations
equations = [oc.compose_equations]
```

## Computational Chemistry doesn't have a standardized output file format

* Need to convert ot single format
* Trying to move to Chemical JSON (CJSON)
    * MolSSI is moving to make it standard

## Data Management 
* Girder
    * Web based data management platform
  
## Job Execution
What's involved in submitting to HPC

* Input Generation
* Moving data onto the resource
* Generate Submission Script
* Submit and Monitor obs
* Post-Processing and ingestion of result

They want to focus on shielding end-users from these complexities

## Job Execution
* SGE, PBS, Slurm (+NEWT)
* Template input decks
* Distributed task queue to support long running operations
    * Job submission and monitoring
    * Support "offline" execution of Jobs

## Notebook Management 
* JupyterHu to enable multi-user environment
    * DockerSpawner
        * User does not need account on server
        * Simple Deployment of Complex Jupyter configs
* Jupyter/Girder integration

## Notebooks as data

* The notebooks encode the workflow 
* Store int the data management system along with the output
* Girder Contents Manager

## Frontend

Uses JupyterLab + extensions

* allows creation of new custom reusable encapsulated HTML tags
* some other js
* Mime render
    * react/redux stack 
* typescript

## Deployment 

* Docker compose
* Ansible for runtime configs
* AWS
* NERSC National Energy Research Scientific Computing Center
    * Jobs run on Cori (10th fastest super computer)

## Future Work

* Extend collaboration Features
    * Fork notebook
    * Realtime editting of notebooks
* Integrate more computational and materials codes
    * psi4 , NWChemEX, Orca
* Add machine learning capabilities
    * Bulk Downloads for training datasets
* Semantic Web
    * Enriching data and making it more discoverable
