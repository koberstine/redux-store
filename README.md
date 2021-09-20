[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

# Redux Store

## Description

This project takes an existing eCommerce application, utilizing Global State through React's Context API, and migrates the application to Redux. The migration utilizes npm packages redux and react-redux. There is much debate over Global State vs 'Prop Drilling' and Context vs Redux. While passing props can sometimes be cumbersome to code, there is no package footprint, making the code inherantly more stable. They also enforce a one-way, tracable path through the code. Switching to a Global State (which was done to this app via Context prior to migrating to Redux) aleviates difficulties when your components do not have a direct parent/child relationship. However, this comes at a cost of adding packages to the application, which could reduce responsiveness. Context is considered by many to be more desirable for small applications where changes to state are minimal. The reason is that Context rerenders on any change to state. There are situations where using multiple contexts can avoid unessisary rerendering. Typically, opinion is that Redux would be more apropos a larger application. This is largely because of the need for additional libraries, but Redux does allow for only rerendering updated components which is ideal for high frequency state changes.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Credits](#credits)
- [Deployed-App](#deployed-app)
- [Screenshot](#screenshot)
- [License](#license)
- [Contributing](#contributing)
- [Tests](#tests)
- [Questions](#questions)

## Installation

Download source files, navigate in console to main project directory, run 'npm install' and 'npm run seed'

## Usage

Navigate in console to main directory of project, run 'npm run start' to run the application on Local Host. The 'start' script in package.json will detect a development environment and use 'start:dev' or a production environment and use 'start:prod' there is also a 'heroku-postbuild' script for deployment to Heroku. Once deployed on Heroku and connected to MongoDB Atlas, use 'heroku run npm run seed' to seed the datatbase.

## Credits

Starter code provided by UCF Coding Boot Camp, University of Central Florida. Migration to Global State using Context API accomplished using step-by-step instructions provided by UCF Coding Boot Camp. Migration to Redux done by Chris Koberstine.

## Deployed-App

https://murmuring-brushlands-08289.herokuapp.com/

## Screenshot

![](https://github.com/koberstine/redux-store/blob/main/screenshot.jpg)

## License

[https://www.mit.edu/~amini/LICENSE.md](https://www.mit.edu/~amini/LICENSE.md)

    MIT License

    Copyright (c) [2021] [Chris Koberstine]

    Permission is hereby granted, free of charge, to any person obtaining a copy
    of this software and associated documentation files (the "Software"), to deal
    in the Software without restriction, including without limitation the rights
    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
    copies of the Software, and to permit persons to whom the Software is
    furnished to do so, subject to the following conditions:

    The above copyright notice and this permission notice shall be included in all
    copies or substantial portions of the Software.

    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
    SOFTWARE.

## Contributing

No contributions to this project are being accepted at this time

## Tests

No tests have been written for this project

## Questions

Github: [koberstine](https://github.com/koberstine/)

Please submit any additional questions via email to <koberstine@hotmail.com> with 'github.com/koberstine/redux-store' in the subject of the email.
