# Project. Restaurant App: Stage 1

---
### Udacity Front-end Development Nano-degree

### Google Scholarship

## Table of Contents

* [1. Introduction: Restaurant Reviews](#introduction)
* [2. Restaurant Reviews project and its objectives](#objectives)
* [3. How to run the app?](#howtorun)
* [4. What objectives have been achieved?](#objectivesachievement)
* [5. What is required to run the app?](#requirements)
* [5. Contributing](#contributing)

---

## 1. Introduction: Restaurant Reviews

The **Restaurant Reviews** is an app that allows to check the near-by restaurants and read opinions about them. The user can check where is the restaurant, what time it is open and check how other visitors rated it. The user can see the locations of the restaurants directly on the map. Thanks to it, he can check the near-by restaurants and choose the best one for him!

## 2. Restaurant Reviews project and its objectives
The main objective of the **Restaurant Reviews** projects was to incrementally convert a static webpage (the basic scripts were delivered) to a mobile-ready web application. In **Stage One**, it was requested to take a static design that lacks accessibility and convert the design to be responsive on different sized displays and accessible for screen reader use (smartphones, tablets, etc.). Also, it was needed to a service worker to begin the process of creating a seamless offline experience for users.

## 3. How to run the app?
To run the app, you need to start up a simple HTTP to serve up the site files on your local computer.Python has some simple tools to do this. In a terminal, check the version of Python you have: `python -V`. If you don´t have Python installed, navigate to Python's [website](https://www.python.org/) to download and install the software. Then, follow below steps:
1. Fork and clone the this repository.
2. Open a terminal and from from inside the new directory, launch a local client server using Python from your terminal:
* `Python 2: python -m SimpleHTTPServer 8000`
* `Python 3: python3 -m http.server 8000`
3. Open the browser and check the site at `http://localhost:8000`.

Great! Your app should run!

## 4. What objectives have been achieved?
Within the project objectives, we can list following challenges:
* Make the side fully responsive
* Make the site accessible
* Cache the static site for offline use

Below description how those goals have been achieved

### 4.1. Responsive design
The viewport has been implemented for `index.html` and for `restaurant.html`. Also, the breakpoints have been determined depend on the device resolution. Thanks to it, the images do not overlap, and page elements do not wrap when the viewport is too small to display them side by side. Moreover, the `Grunt` plugin has been used to optimize the image assets used in  app project.

### 4.2. Accessibility
The next challenge was to achieve a high accessibility between 90% and 100%. In order to it, the script has been improved to add the `alt` to all images that did not have it. Also, other design aspects have been improved, like a contract of colours, descriptions, semantic markups, etc.

### 4.3. Offline access
The project objective was to make a website accessible offline. Using Cache API and a ServiceWorker, cache the data for the website so that any page (including images) that has been visited is accessible offline. In this case, very helpful was Google Dev article (videm: https://developers.google.com/web/fundamentals/codelabs/offline/) that explains very well how to register Service Worker, how include it in the scripts, how to create a cache store and - how to test it.

## 5. What is required to run the app?
To run the app, several setups and installation are required:

#### 1. Mapbox
You will need a MapBox API key. Replace the text <your MAPBOX API KEY HERE>inside of main.js with your key. MapBox API is free to use, without providing any payment information. You can register [here](www.mapbox.com).

##### 2. Grunt
For optimizing images, we use Grunt. You can set it up using following instruction: [Getting started with Grunt](https://gruntjs.com/getting-started). Also, you need to have installed:
* [gulp-jimp-resize](https://www.npmjs.com/package/gulp-jimp-resize)
* [gulp-image](https://www.npmjs.com/package/gulp-image)
* [bluebird](https://www.npmjs.com/package/bluebird)

## 6. Contributing

This repository is the starter code for _all_ Udacity students. Therefore, we most likely will not accept pull requests.

For details, check out [CONTRIBUTING.md](CONTRIBUTING.md).
