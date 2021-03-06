---
heading: FreshBooks
seo: Overview | FreshBooks | Cloud Elements API Docs
title: Overview
description: Integrate FreshBooks into your application via the Cloud Elements APIs.
layout: docs
breadcrumbs: /docs/elements.html
elementId: 172
parent: Back to Element Guides
order: 1
sitemap: false
---

## Welcome to the FreshBooks Element


#### At a Glance

In order to create a connection to FreshBooks the following steps are required:

1. Register as a [consumer](freshbooks-endpoint-setup.html)
2. Call the `GET /elements/freshbooks/oauth/token` with your FreshBooks API key, secret, and siteAddress
3. Call the `GET /elements/freshbooks/oauth/url` with your FreshBooks API key and secret, requestToken, and siteAddress
4. Call the `POST /instances` API to instantiate your FreshBooks connected app

#### In Depth

The FreshBooks Element is a collection of resources providing a pre-built integration into a service endpoint. RESTful methods (POST, GET, PUT, PATCH, DELETE) are used to interact with these resources (accounts, contacts, files) regardless of the type of APIs (SOAP or REST) provided by the endpoint. Elements leverage Cloud Elements API Manager platform services including authentication, data transformation, and event management.  The API is built to allow you to create a functional application or integration quickly and easily.

All API calls to Cloud Elements should be made to the `https://api.cloud-elements.com/elements/api-v2` base domain. Requests are authorized with an Organization and User secret, as well as, an Element token.  We use many standard HTTP features, like HTTP verbs, which can be understood by many HTTP clients. JSON will be returned in all responses from the API, including errors. The APIs are designed to have predictable, straightforward URLs and to use HTTP response codes to indicate API errors.

Get started by [registering as a consumer](freshbooks-endpoint-setup.html).
