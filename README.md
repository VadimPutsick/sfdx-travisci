# Conference Application

## Table of contents

* [Installation instructions](#installation-instructions)

## Installation Instructions

### Installing Conference using Salesforce DX
This is the recommended installation option for developers who want to experience the app and the code.

1. Install Salesforce DX. Enable the Dev Hub in your org or sign up for a Dev Hub trial org and install the Salesforce DX CLI. Follow the instructions in the [Salesforce DX Setup Guide](https://developer.salesforce.com/docs/atlas.en-us.sfdx_setup.meta/sfdx_setup/sfdx_setup_intro.htm?search_text=trial%20hub%20org) or in the [App Development with Salesforce DX](https://trailhead.salesforce.com/modules/sfdx_app_dev) Trailhead module.

If you don`t login in your dev org execute nex command
sfdx force:auth:web:login -d -a PartyOrganizer

1. Clone the **conference** repository:
    ```
    git clone https://github.com/VadimPutsick/corporate-party-organizer
    cd corporate-party-organizer
    ```

1. Build project in new scratch org:
    ```
    sfdx force:org:create -s -f config/project-scratch-def.json -a corporate-party-organizer

1. Push metadata in your scrath org:
    ```
    sfdx force:source:push

1. Open the scratch org:
    ```
    sfdx force:org:open
    ```