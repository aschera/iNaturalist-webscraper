# iNaturalist Web Scraper

## Introduction

In this project, we will build a web scraper using Python to download images and metadata from iNaturalist. The project, called `iNaturalist-webscraper`, is designed to extract images and associated metadata for specific taxa and save them locally for further analysis. This guide will walk you through the steps to set up the scraper, run it, and manage the downloaded data.

## Prerequisites

Before starting, ensure you have the following:

- Python installed on your system
- Basic knowledge of Python programming
- The following Python libraries installed:
  - `BeautifulSoup` for parsing HTML
  - `requests` for making HTTP requests
  - `xml.etree.ElementTree` for creating XML files
  - `os` for interacting with the operating system

You can install the necessary libraries using pip:

```bash
pip install beautifulsoup4 requests

# Project Structure
Your project directory should be structured as follows:

iNaturalist-webscraper/
├── data/
│   ├── websites/
│   └── <taxon_id>/
├── scraper.py
└── README.md

- data/websites/ will contain the HTML files of the web pages we scrape.
- data/<taxon_id>/ will contain the downloaded images and their metadata for each taxon.
- scraper.py is the main script that runs the scraper.

