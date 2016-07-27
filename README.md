# Frontend Development Test: Tree structure of subjects

In [subjects.csv](subjects.csv) (also available as [subjects.json](subjects.json)) you will find a list of subjects that are part of our History learning method (_Leswijs Geschiedenis_). 
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

## Use case for this test

A teacher is looking for learning material and has some notion of what the learning material should be about.
The teacher is unaware of the precise subjects that we have in our database. 
The teacher should be able to select multiple subject for which he/she would like to see the learning material. 

## Test

1. Create a tool for teacher to use to select one or more subjects (from [subjects.csv](subjects.csv)), 
so that it can be used by teachers to filter our learning material.  
In the example above the user should be able to select for example *Homo sapiens* and *Egyptenaren* to find all learning material that is about those subjects.
2. Make a separate list of the selected subjects. This is the list that would be send to a backend service to retrieve learning material on those subjects.

## Frameworks
You can use any _framework_ (VanillaJS, AngularJS, EmberJS, ReactJS, BackboneJS, ...) to get this done. Please don't use jQuery plugins (at Dedact we use [BackboneJS](http://backbonejs.org/) and its _events_, _models_ and _collections_).

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


