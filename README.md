# IIGB website content

<!-- toc -->

- [The purpose](#the-purpose)
- [Getting Started with development](#getting-started-with-development)
  * [Get the source](#get-the-source)
  * [Project/File Structure](#projectfile-structure)
- [Deployment & Release](#deployment--release)

<!-- tocstop -->

## The purpose
This repository contains the webiste content for the great and IIGB websites in a format that can be pulled in by the website as a node module and used by metal-smith to build out the static pages that make up the site.

## Getting Started with development

### Get the source
Run the following from the command line to download the repository and change into the directory:

```bash
git clone git@github.com:uktrade/iigb-beta-content.git

cd iigb-beta-content
```

### Project/File Structure

Below snippet outlines project structure. This snippet only lists files of importance.

```
- content/
  - _labels/                #Contains nav headings, button text etc. for the IIGB website
  - _labels-great.gov.uk/   #Contains nav headings, button text etc. for the great website
  - beta/                   #Contains page content for IIGB website
  - great.gov.uk/           #Contains page content for great website
- geoip/                  
  - country_redirects.json  #Defines the mapping of IP geo locations to the languages used in the website.
- media/                    #Contains all the images used across the site.
- _prose.yml                #Defines the folder structure for the repository.
- package.json        
- README.md           

```

## Deployment & Release

Branch `staging` is continuously deployed to [staging environment](https://staging.invest.great.gov.uk/) for QA purposes, using the current version of the `develop` branch for the iigb-beta-website repository.
