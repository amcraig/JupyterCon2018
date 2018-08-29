# SWAN: CERN's Jupyter-Based Interactive Data Analysis Service

Diogo Castro: Full Stack Developer for CERN

[Swan Link](http://swan.web.cern.ch/)

## Workflow for HEP-CERN:
DataCollect from ATLAS/ALICE/CMS/LHCb
|
Raw Data 1GB/sec
|
Reconstructed
|
Processing
|
Analysis
|
Results

## Goal: to scale 10x more collisions, 30x more data

## Problem: Workers used to download data to personal computers to do work, but as this scales a web app makes the most sense.

## Solution: build a data analysis solution with a C++ kernel and Jupyter and integrate with other CERN tools 
(Synergy beween ROOT(CERN Data analysis), R, Python, etc)

## Integration:
* Infrastructure
    * Docker
    * Jupyter
* Storage
    * CERNBox (SWAN's shared home directory)
    * EOS (Disk Storage System)
* Software
    * CERNVM File System (CVMFS is a software distribution service that minimizes the size of Docker containers)

Multiple Kernels available: Python 2 or 3, ROOT C++, R, Octave

## Leveraging the Power of Jupyter(Hub)

There's a new user interface that allows you to spin up your instance with desired resources: Kernels, Cores, Platform, File System

## Collaborative Analysis

Full integration with their dropbox

Apache Spark Cluster adoption for analytics visualization
Integrates with: 
* Spark Connector (By CERN - configure all connections)
* Spark Monitor
    * Lets you see progress bars for jobs
    * task timeline
    * resource utilization

## Outreach 
Scientists and all higher education around the world

## Future work
Full integration for Jupyter lab WHICH means all visualizations will move to all JavaScript based

[Repo](https://github.com/swan-cern)

[Science Box](cern.ch/sciencebox)

## Take aways:
Jupyter is now serving as an entrypoint for CERN's Computing Resources and Data

# Fun Facts:
* Most CERN Employees don't use a terminal, or Git
