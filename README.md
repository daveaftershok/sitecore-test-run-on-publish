# Sitecore run tests on publish

- Run UI tests (via cypress test runner - http://cypress.io) on a publish to staging publishing target.
- Tests validate the publish has not broken key areas of the website.
- If a content editor then wishes to publish to a live target they have an indication that the latest changes will not have an adverse affect on the site.

![howitworks](https://raw.githubusercontent.com/daveaftershok/sitecore-test-run-on-publish/master/result.gif)


## Dependencies

This code requires cypress-node-api-windows (https://github.com/daveaftershok/cypress-node-api-windows) to be running.

## To setup:

Pick the correct version of publish.js and overwrite the version in your sitecore solution. Pick the correct file based on your Sitecore version. If you version isn't listed take the code from the v9 folder and update your sitecore\shell\Applications\Dialogs\Publish\publish.js with the custom code between the START and END comments.

## To configure and run:

- Enure you are running the Cypress API.
- update a couple of configuration variables:
-- testRunnerHost - The node api location
-- stageTargetName - The name of your stage publishing target

