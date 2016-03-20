
# FrisbyJS

[FrisbyJS](https://www.npmjs.com/package/frisby) is a [Jasmine](https://www.npmjs.com/package/jasmine-node) extension that allows us to write acceptance tests for web APIs.

1. start by using terminal to navigate to the `frisbyjs/` directory and run `npm install` to install the module dependencies. You will need to install **jasmine-node** globally if this has not already been done.
2. open the `todo-spec.js` script and read it, paying particular attention to the detailed comments.
3. start the API and check it is visible using Postman.
4. change the base urls to match your cloud9 API.
5. run the acceptance tests by entering `jasmine-node test/ --verbose`, this will output the test results to the terminal. Take a few moments to understand this output.
6. run the acceptance tests again. Why do they fail this time, use the error trace to find out what failed and why.

## 1.1 Test Your Knowledge

1. create a new test `DELETE /lists` and add it at the start of the test. Eventually this should clear all the lists in the API and return success, lists deleted.
2. run your tests, they should fail (we have not written the new API feature!
3. add the  `--autotest --watch .` flags when you run the test script (see the previous worksheet), this will automatically run your acceptance tests every time you save a file.
3. implement `DELETE /lists`. The tests will pass to indicate success.
