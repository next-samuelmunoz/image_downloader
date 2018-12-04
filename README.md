# Image Downloader

## Description
This tool allows to download the images from a query from different search engines.


## Features
* Firefox as web browser.
* Headless mode, the web browser is not visible.
* Modular code, easy to add new search engines.
* Sources:
  *  Google Images


### TODO
*  Implement a fast image downloader. Parallel from different hosts.


## First steps

### Requirements

* firefox (tested with version 59.0.2 in Ubuntu 64bit).
* make
* python3 (tested  with version 3.5)
* virtualenv
* tar

### Installation
```bash
git clone https://github.com/beeva-samuelmunoz/image_downloader.git
cd image_downloader
make install
```

*Note: if you want to use other python version rather than 3.5, type:*
```bash
make install PYTHON_VERSION=<version>
```

### First run
Once in the project folder `image_downloader`.
* To get some help type:
```bash
make
```
* Example, download images of *red cars* from Google Images.
```bash
make dl_google query="red cars"
```
  * *Note: the images will be downloaded under the path:*  `image_downloader/data/red car-google`.
