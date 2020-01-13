# poc-coveo-search
Proof of concept using coveo search JS framework

To run this example is necessary to have installed Node Js. Go to the folder where the project was cloned, then open a terminal or open folder at Visual Studio Code, place at main folder and run the following commands:
- npm install
- npm run build
- npm run watch

Sometimes is not possible to run the server because the trial version of the organization needs to be updated or the api keys are expired. If you want to play with example sources provided by coveo comment script at head and replace it with this:
      
      document.addEventListener('DOMContentLoaded', function () {
        Coveo.SearchEndpoint.configureSampleEndpointV2();
        Coveo.init(document.body);
      })
      
If you want to index your own sources you have to create a trial account at coveo search organization, you will need to send a post with this Swagger UI https://platform.cloud.coveo.com/docs?api=Platform#!/Organizations/rest_organizations_post copy the OrganizationId from the response and then go to https://platform.cloud.coveo.com/login and log in with whatever you want, own coveo acc. or google acc. You will have to sync your acc with the organization id and then start adding sources and wait while coveo build them. For more information refer to https://docs.coveo.com/en/402/javascript-search-framework/javascript-search-framework-tutorial-5-configuring-your-own-search-endpoint

For full tutorial from scratch refer to: https://docs.coveo.com/en/301/javascript-search-framework/javascript-search-framework-tutorial-0-environment-setup where you can follow step by step how coveo search works
