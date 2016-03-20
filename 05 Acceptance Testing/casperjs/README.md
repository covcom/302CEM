
# CasperJS

[CasperJS](http://casperjs.org) is a NodeJS package that uses the PhantomJS headless web browser to test your websites. This totorial is based on the **Cloud9 IDE**.

## Installation

It requires a recent version of NodeJS to be installed. Updating NodeJS is done using the Node Version Manager (NVM) tool. Once we have installed the latest stable version we run the node command as shown to check the precise version.
```
nvm install stable
node -v
```
Next we need to globally install both PhantomJS and CasperJS. These are available as _NodeJS modules_ and need to be installed globally using the `-g` flag.
```
npm install -g phantomjs
npm install -g phantomjs
```
## Running a Test

Load the web page `basic_math.html` file and use the run button to start the Apache web server. Copy the page URL and assign it to the `url` constant at the top of the `basic-math-spec.js` script page.

Use the _terminal_ to navigate to the directory containing the `basic-math-spec.js` script and run the test suite. Notice the two flags that are used. Find out what they do by reading the [documentation](http://docs.casperjs.org/en/latest/testing.html#test-command-args-and-options) page.
```
casperjs test basic-math-spec.js --concise --fail-fast
```

Try omitting the flags, what happens? Try using some of the other available flags and note the effect they have on the output.

## Test Your Knowledge

1. The test suite covers all the functional requirements including:
  - Applying a discount
  - Doubling the discount for orders of over 100 units
  - Shipping charges
2. Implement the requirements based on the instructions in the worksheet.
3. Run the acceptance tests regularly to monitor your progress.
4. When all the tests pass you have completed the web app, congratulations!

## Apply Your Knowledge

You have seen a simple acceptance test. Make sure you understand how the acceptance tests are written (syntax). There are two additional acceptance test suites to try out. These demonstrate how to test the majority of website features.

1. Create acceptance tests that demonstrate the current functionality of your website.
2. Create acceptance tests to describe the next user story you plan on implementing.
3. Use the complete suite of tests to demonstrate your next user story has been implemented successfully.
4. Run manual tests to prove your acceptance tests were comprehensive.
