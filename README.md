# APIPCS Gateway management

## Purpose

This API collection updates a deployed API Gateway with new user credentials.

## Setup

1. Set the collection variables. 

- {{Username}} should be set to the gateway runtime user. 

- {{Password}} should be set to that user's password. 

- {{IP}} should be set to the IP address of the instance where your gateway is deployed.

- {{AppId}} should be set to the IDCS application ID

- {{Secret}} should be set to the IDCS secret

2. Obtain your auth token. In the Authorization tab, select "Get New Access Token". Leave the settings as they are and request a new token, then use it.

## Send the API calls

1. Send the "Gateway Runtime" request to update the gateway with the new user credentials

2. Send the "Poll" request to force an update of the gateway, effectively checking the validity of the new credentials.
