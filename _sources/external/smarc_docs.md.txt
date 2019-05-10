smarc_docs
==========

Documentation for the SMaRC project software repositories

## Generating the documentation

### Dependencies

Run `sudo pip install sphinx sphinx_rtd_theme m2r` to get the necessary dependencies.

### Writing documentation

The sphinx tool that generates the docs uses restructured text as input to
generate the pages. See [this page](http://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html)
for details on rst. See e.g. [this example](https://github.com/nilsbore/auvlib/tree/master/docs)
for details on how you can structure the documentation.

### Updating documentation

Go into the root of [this repo](https://github.com/smarc-project/smarc_docs). Run `make html`
and check that all your changes look good by opening `html/index.html` in a web browser.
To get your changes into https://smarc-project.github.io/ there are two options:

#### Easy option

Commit the changes and open a pull request against https://github.com/smarc-project/smarc_docs ,
then ping @nilsbore to do the rest.

#### Hard option

First do the easy step, either by pull request or pushing directly to the repo.
Then copy all contents of the `html` folder into the root of https://github.com/smarc-project/smarc-project.github.io . Commit the changes to that repo and push or open a pull request to get the changes up to https://smarc-project.github.io/ .
