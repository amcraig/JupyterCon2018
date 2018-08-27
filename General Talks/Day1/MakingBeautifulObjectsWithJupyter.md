# Making beautiful objects with Jupyter

[M Pacer](https://mpacer.org/): Senior Notebook Engineer - Netflix

[Slides](https://bit.ly/beautifulObjectJupyterCon)

>Jupyter displays a rich array of media types out of the box. M Pacer explains how to use these capabilities to their full potential, covering how to add rich displays to existing and new Python classes and how to customize the way notebooks are converted to other formats. You’ll learn what MIME types are and how to use them, explore Jupyter’s display mechanisms and protocol, and dive into nbconvert. These skills will enable you to make beautiful objects with Jupyter.

Topics include:
* How to enhance the display objects and classes in the notebook
    * By adding metadata to any output via IPython.display
    * By adding custom repr methods
    * By using updatable displays
* Libraries that enable new kinds of displays, including:
    * vdom: A Python library for React-like declarative layouts
    * display_xml: A Python library for displaying highlighted, indented XML
* How to convert notebooks into custom objects using nbconvert, which allows:
    * Hiding prompts and code cells to show only the output figures
    * HTML where you can toggle whether individual code cells are visible
    * PDFs with support for non-Latin alphabets

***

# Presenter went to fast for very effective notes

## Functional Beauty vs Aesthetic Beauty
* Great example: Text 
* Functional, but people are still making new beautiful fonts

## Custom reprs in Python
* __repr__
    * controls how the object is represented
* __str__
    * how object is transformed to a string
* ANSI excape strings
* No way to support richer types of media

## Media Types:
Previously called MIMEtypes
* Multipurpose Internet Mail Extention
* Each cell can have multiple outputs
* Each output can have multiple media types 
* Each media type can have data & metadata
    * metadata is stored per output
* Front-ends use richest supported media type
* Front-ends may not support some media types

## Built in IPYTHON diplay format
```python

```

allofplos: gives access to all PLOS articles

