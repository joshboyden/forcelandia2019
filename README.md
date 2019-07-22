# forcelandia2019

## Setup
1. Install the [Heroku CLI](https://devcenter.heroku.com/articles/heroku-cli).

1. Install the [Salesforce CLI](https://developer.salesforce.com/tools/sfdxcli).

1. Log into the four orgs you'll use with the Salesforce CLI and give them aliases:

    - **Dev Hub (e.g.. "HubOrg")**: this will create scratch orgs for your Review Apps
    - **Development Org (e.g. "DevOrg")**: this is the first environment you'll update using a package deploy
    - **Staging Org (e.g. "TestOrg")**: this is the first environment from which you'll promote your code via release phase
    - **Prod Org : "ProdOrg"**: this is your production org

    Note: you could cheat and, simply for demo purposes, use the same org for the DevOrg, TestOrg, and ProdOrg.

1. Ensure you see all four orgs when you run `sfdx force:org:list`.

1. Clone and own [setup.sh from Heroku Salesforce Buildpack repo](https://github.com/heroku/salesforce-buildpack/blob/master/scripts/setup.sh) to create pipeline

1. Create a sfdx project. `sfdx force:project:create --projectname forcelandia2019`

1. Create a simple LWC cmp. `sfdx force:lightning:component:create --type lwc --componentname helloForcelandia --outputdir force-app/main/default/lwc`

1. Create a package. 

## Sources 
"Standing on the shoulders of giants"
* https://github.com/wadewegner/salesforce-dx-pipeline-sample