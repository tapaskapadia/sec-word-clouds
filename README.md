# sec-word-clouds
Website generated from scraping SEC filings and visualizing the data as word clouds
https://tapaskapadia.github.io/sec-word-clouds/

## About The Repository
This repository builds and deploys a static hugo generated website on [GitHub Pages](https://tapaskapadia.github.io/sec-word-clouds/). It utilizes a SEC scraper script that can be found  [here](https://github.com/tapaskapadia/sec-forms-word-cloud-script) to pull new SEC filings every weekday automatically utilizing Github Actions. 

Regardless if you are interested in SEC filing visualizations or not, this repository provides a great example of a Github Actions Workflow for automating the building and updating of a website on a regular schedule utilizing an external script to generate new static assets. 
#### How the Github Actions Workflow Works:
1. Checkout  this repository 
2. Checkout an external repository in a different path
3. Installs package dependencies to run the external repository (pip installs)
4. Run the external script which generate static assests (hugo markdown files, images, and json data) to be added to this repository 
5. Commit and Push the static assests to this repository
6. Build the hugo site & Deploy to Github Pages
7. Repeat every weekday. 

Why:
* Why Not

### Built With
Hugo 
Github Actions

