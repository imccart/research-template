
## Research Template Overview

This repo is a template for a research project and companion site. The repo consists of four main areas:

1. the [yaml](_site.yml]) file describes the basic layout of the site, which is a landing page with some tabs along the top of the page. Note that the yaml as currently written anticipates that you host the site as part of GitHub pages and that the site's html files are in the [docs](/docs) folder.

2. The landing page is described in the [index](index.Rmd) file.

3. The rest of the .Rmd files relate to each of the tabs listed in the yaml file. This template envisions four such tabs (data, analysis, appendix, and present). 

4. The subdirectories (analysis, data, data-code, html, presentations, results) house other materials relevant for the repo, as described below:

  - [data](data): the raw data...should be added to your .gitignore file
  - [data-code](data-code): code files for data management (no analysis here)
  - [analysis](analysis): code files for analysis (anything that goes into the actual paper)
  - [results](results): output and potentially log files from the analysis, with subdirectories for figures and tables
  - [presentations](presentations): all files necessary to build different presentations of the paper
  
  
## Directions for Use

Recall, [_site.yml](_site.yml) tells Rstudio how to build the site - particularly, that the site should go into the "docs" folder. To deploy the companion site, follow these steps:

1. Enable github pages

2. Build site with the build site button or rmarkdown::render_site()

3. Push changes to github. Note, if you're using a custom site for github pages, then github creates a new "CNAME" file, which you'll need to pull. This gets deleted every time you recreate the docs folder, so just be careful not to push the deleted file to github!


--------------------------------------------------------------------------------

**Ian McCarthy**  
Department of Economics • Emory University<br>
Faculty Research Fellow • National Bureau of Economic Research<br>
[ianmccarthyecon.com](https://www.ianmccarthyecon.com) • [\@ianhealthecon](https://twitter.com/ianhealthecon)
