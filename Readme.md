# Introduction to python Spring 2022

## Elective at KEA CS 4th semester.

**View Online:** https://python-elective-kea.github.io/spring2022/

Or **view local** by cloning this repository

````
  git clone https://github.com/python-elective-kea/spring2022.git

````
Open the index.html page in the "sphinx -> build" folder and use the website.


## Working with the source files

If you want to work with the source files

### Run in docker container

````

$ docker run --rm -v /path/to/document:/docs sphinxdoc/sphinx make html

````

### Install Sphinx

````
  $ pip install -U sphinx

````

And read the documentations here: https://www.sphinx-doc.org/en/master/contents.html  

The source files can be found in "sphinx -> source" folder.

The "build" files are identical with the ones in the "docs" folder, but are used for local display.

