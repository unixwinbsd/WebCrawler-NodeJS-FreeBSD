# Web Crawler CLI Node JS On FreeBSD
A simple web crawler CLI that takes a URL as input and outputs all the links on the website, ordered by no. of occurrence. The output is seperated into internal and external links and exported to .csv files.

## Description
This CLI application crawls the base URL, which the user provides, as well as all its subpages. The NodeJS web crawler then divides the links into internal and external links. Internal links are links that point to other pages on the same domain. External links are links that lead to other domains on your website. For each link, it counts the number of occurrences and displays the final result in descending order. The output is split into internal and external links and printed to the terminal, where it is saved in a .csv file.

## How to use it

### Prerequisits
You must have Node.js installed on your computer. This project was developed using Node.js v18.7.0
node -v - to check your node version
nvm run  
### Installation
Clone the repository to your computer and run the following command in the root directory of the project to install the dependencies:
``` bash
npm ci
```
#### In case of problems with the installation
If you encounter any problems with the installation, first check whether you're using a matching Node.js version: `node -v`
This project was build with node V18.7.0. If you use nvm, run `nvm run` to switch to the correct version.

If your Node version isn't an issue, try deleting the package-lock.json file, and reinstall the dependencies by running the following commands:

``` bash
npm init  # to initialize the project
npm install jest --save-dev  # to install jest for testing
npm install jsdom
npm install json2csv
```
### Usage
Run the “npm start” command to start the NodeJS Web crawler.
``` bash
npm start 
```
Then simply follow the instructions.
This program will ask for the URL that you want to crawl. Enter the URL you want to browse. The program will then crawl the URL and all its subpages. The results will then be output to the terminal and exported to a .csv file. The file will be saved in the reports directory.

## How to Contribute
Contributions are always welcome! Please check the Code of Conduct .

## License
This project is licensed under the MIT License.

## Support
If you have questions or need help getting started, please open an issue in the repository. Or if you are confused about how to learn it, please visit https://www.unixwinbsd.site
