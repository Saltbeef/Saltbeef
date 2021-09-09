# Garden

## Links

* [Getting started](https://squidfunk.github.io/mkdocs-material/getting-started/)
* [Mastering Markdown](https://guides.github.com/features/mastering-markdown/)
* [MkDocs configuration](https://www.mkdocs.org/user-guide/configuration/)


## Local setup

* Copy SSH public key to your Github settings [Settings / Keys](https://github.com/settings/keys)
* Clone it `git clone git@github.com:Saltbeef/Saltbeef.git`
* Create a python virtual environment using Poetry `poetry init -no-interaction` 
* Install the package `poetry add mkdocs-material`
* Generate and publish the documentation `poetry run mkdocs gh-deploy`

## Setup pipeline

* Copy mkdocs.yaml from [onedr0p's home-cluster](https://github.com/onedr0p/home-cluster/blob/main/mkdocs.yaml)
* Rip out all extras and plugins
* Create .github/workflows/mkdocs.yaml and populate with the [example code](https://squidfunk.github.io/mkdocs-material/publishing-your-site/#github-pages)
* Commit the changes


## Hostname

Create a CNAME record in the Cloudflare dashboard that points to saltbeef.github.io (DNS only)


## Github pages

Go to [Settings / Pages](https://github.com/Saltbeef/Saltbeef/settings/pages)

* Set branch to gh-pages, root is /
* Set Custom Domain to garden.barren.land
* SSL cert will take a while to be generated
* Enable Force HTTPS once it is there

