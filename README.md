# Sitecore run tests on publish

- Run UI tests (via cypress test runner - cypress.io) on a publish to staging publishing target.
- Tests validate the publish has not broken key areas of the website.
- If a content editor then wishes to publish to a live target they have an indication that the latest changes will not have an adverse affect on the site.



## Dependencies

This code requires cypress-node-api-windows (https://github.com/daveaftershok/cypress-node-api-windows) to be running.

### To setup:

Pick the correct version of publish.js based on your Sitecore version. If you version isn't support take the code from Sitecore 9 and update your sitecore\shell\Applications\Dialogs\Publish\publish.js with the code.

## To configure and run:

- Enure you are running the Cypress API.
- update a couple of configuration variables:
-- testRunnerHost - The node api location
-- stageTargetName - The name of your stage publishing target

