![baloo-logo](https://user-images.githubusercontent.com/108659858/177123891-25e143bd-3221-463e-b98f-af1f121a9f4c.png)

_Baloo is the modern learning management system (LMS) that enables organisations and individuals to create, certify and sell knowledge to anyone on the web. Find out more at our website; [https://www.baloolearning.se](https://www.baloolearning.se)._

# Baloo external API
This repository contains developer instructions for using the Baloo external API — a RESTful integration for third parties to consume and modify Baloo data. The feature is currently an add-on service that needs to be specifically enabled by your customer representative for your Baloo workspace.

# How can we access the extrenal API?
Once the external API has been enabled for your workspace you will need to sign in to the Baloo dashboard as an administrator and create an access key. You do this by navigating to the `Configure` app and scrolling to the very bottom. Here you will be able to generate a total of two unique access keys. These will only be available upon creation so make sure to save the generated key in a safe space. If you loose the key you can at any point revoke the key and create a new one.

With your access key ready you will be able to send requests to the external API endpoint `http://customer-api.baloolearning.se/v1/` by including it as an authorization bearer token. For example:

````
GET: http://customer-api.baloolearning.se/v1/users
Headers:
Authorization: Bearer ${accessToken}
````
_This request will return a list of the users currently part of the workspace_

For a list of all currently possible requests, please see the [OpenAPI documentation here](https://customer-api.baloolearning.se/v1/openapi.json).

# Coding examples
Still to come... Do you have any examples you wish to share? Please let us know!

# Next steps...
For support, requests for additions to our available endpoints, or notifications of upcoming chanegs, please feel free to join our Slack workspace, [Baloo Community](https://join.slack.com/t/baloolearninggroup/shared_invite/zt-1c7wiuagw-3JiKfrxAKhDgVfy~VglVng).
