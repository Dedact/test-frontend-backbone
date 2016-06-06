# Frontend BackboneJS Test: Tree structure of subjects

In [subjects.csv](subjects.csv) you will find a list of subjects that are part of our History learning method (_Leswijs Geschiedenis_). 
These subjects have a hierarchical structure: subjects can have _sub_-subjects that are more detailed. 
Subjects with `parent_subject_id === 0` are in the top of the hierarchical tree, and subjects with `parent_subject_id !== 0` have the subject with that `id` as their parent.
For example:

```
- Tijd van jagers en boeren
  - De eerste mensen
    - Evolutietheorie
    - Het scheppingsverhaal
    - Homo sapiens
  - Egyptenaren
    - De cultuur van de Egyptenaren
    - ...
- ...
```

All learning material available in Learnbeat have one or more subjects attached. 
That makes filtering for learning material easy. 
The goal of this test is to make a tool for teachers to use when filtering learning material on subject. 
Instead of showing all the subjects available, display them using the hierarchical structure.
Show a interactive subject tree based on the subjects in [subjects.csv](subjects.csv) select multiple subjects in the tree

## Test

1. Use [BackboneJS](http://backbonejs.org/) and its _events_, _models_ and _collections_ to create an interactive tree 
to select one or more subjects, 
so that it can be used by teachers to filter our learning material based on those subjects. 

_In the example above the user should be able to select for example *Homo sapiens* and *Egyptenaren* 
to find all learning material that is about those subjects._

2. Make a separate list of the selected subjects. This is the list that would be send to a backend service to retrieve learning material on those subjects.

## Assessment

You will be assessed on:

* user interaction / user experience
* code quality 
* performance

## Submit your test

Send an email to frank@dedact.nl with:
- all relevant files attached in a Zip archive
- a file describing your thought process
- the amount of time you used to create your submission


