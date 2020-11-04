<img src="https://user-images.githubusercontent.com/11653294/64466233-7cd17480-d119-11e9-8965-e036c1e23c9a.png" alt="CF logo" height="150" align="left"/>

# SAP Cloud Platform Alert Notification Client
>*Promise based Node.js client library to support the usage of SAP Cloud Platform Alert Notification service*

[![Documentation](https://img.shields.io/badge/Service_Documentation-@SAP%20Help%20Portal-ff9900.svg)](https://help.sap.com/viewer/product/ALERT_NOTIFICATION/Cloud/en-US)
[![Blog](https://img.shields.io/badge/Service--related_Blogs-@SAP%20Community%20Portal-3399ff.svg)](https://blogs.sap.com/tag/sap-cloud-platform-alert-notification/)

## About
SAP Cloud Platform Alert Notification is part of the DevOps portfolio of the SAP Cloud Platform. The service is specialized in instant delivery of events coming straight from the core platform services, e.g. database or application monitoring tools. This way you're always the first one notified whenever an issue with your dependency occurs. Additionally, Alert Notification provides means for posting real-time
crucial events directly from your application. All those events altogether - either your custom events, or the platform ones, could be received on whatever channel is preferred - e-mail, Slack, custom webhook, etc.
Furthermore, events can be even stored in Alert Notification storage and pulled from it later.

### Features

* Post custom events
* Pull already stored events either custom, or platform events, and on the other hand, either stored by request, or stored because the requested action has failed for some reason
* Manage your actions, conditions and subscriptions

### Installation

```bash
$ npm i alert-notification-node-client
```

## Getting started

In order to get started visit the [documentation page](TODO:githubpages).

Here is a simple example on how to import and create your client:

```js
import {
    AlertNotificationClient,
    EntityType,
    BasicAutentication,
    RegionUtils,
    Severity,
    Category
} from 'sap-cloud-platform-alert-notification-client';

const client = new AlertNotificationClient({
    authentication: new BasicAuthentication({
        username: '<your-technical-client-username>',
        password: '<your-technical-client-password'
    }),
    region: RegionUtils.EU10;
});

// After that you can use the provided methods from the alert notification instance
```

### Have an issue?
Please, let us know by filing a [new issue](https://github.com/sap-staging/clm-sl-alert-notification-client/issues/new).

### Contributing
We're always open for improvements! If you think the library could be better, please, open an issue and propose your solution as a pull request. We will contact you for discussion as soon as possible.

### License
This project is run under the licensing terms of Apache License 2.0. The paper could be found in the [LICENSE](https://github.com/sap-staging/clm-sl-alert-notification-client/blob/master/LICENSE) file
in the top-level directory.

