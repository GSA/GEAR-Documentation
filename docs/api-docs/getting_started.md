---
layout: default
title: API Basics
nav: basics
---

### Getting Started

The current version of the API lives at ```https://ea.gsa.gov/api/...```

- These endpoints each return a list of objects, or can be limited to a particular {id}.
- Some endpoints have further attributes that bring back other objects related to that {id}. 
- A [Glossary of GEAR terms](https://ea.gsa.gov/#/glossary) can help define some of these objects. (You will need to be on the GSA network to reach the glossary) 

#### Versions

| Version | Date | Changes | 
| ------------- | ------------- | ------------- |
| ```version 1``` | 09/25/2020 | Updates and rewrite of entire GEAR platform
| ```version 0``` | 03/31/2017 | Initial deployment using node.js and Express


#### Endpoints

| Endpoint | What it does |
| ------------- | -------------|
| ```/applications``` | Returns the complete list of GSA Business Applications, to include retired applications
| ```/applications/get/{id}``` | Returns one Business Application by {id}
| ```/applications/get/{id}/capabilities``` | Returns the Business Capabilites and Business Capability metadata associated to the indicated Business Application {id}
| ```/applications/get/{id}/technologies``` | Returns the IT Standards and IT Standards metadata associated to the indicated Business Application {id}
| ```/applications/applications_retired``` | Returns the list of all retired GSA Business Applications
| ```/applications/latest``` | Returns the most recently created GSA Business Application
| ```/applications/statuses``` | Returns the list of possible application statuses
| ```/applications/host_providers``` | Returns the list of possible host providers for GSA Business Applications

| ```/apptime``` | Returns all entries for TIME analysis of all Active GSA Business Applications
| ```/apptime/get/{id}``` | Returns all entries for TIME analysis of the indicated Business Application {id}

| ```/capabilities``` | Returns the complete list of GSA's Business Capabilities
| ```/capabilities/{id}``` | Returns one Business Capability indecated by {id}
| ```/capabilities/{id}/applications``` | Returns the Business Applications that are related to the Business Capability identified by {id}
| ```/capabilities/sso/{name}``` | Returns the Business Capabilities that are related to the SSO organization identified by {name}

| ```/data_flow``` | Returns the complete lit of data flow entries for all GSA Business Applications
| ```/data_flow/get/{id}``` | Returns the Business Applications that interface with the Business Application identified by {id}

| ```/fisma``` | Returns the list of GSA's FISMA Systems, excluding inactive systems
| ```/fisma/{id}``` | Returns one FISMA System identified by {id}
| ```/fisma/{id}/applications``` | Returns the Business Applications and Business Application metadata associated to the indicated FISMA System {id}
| ```/fisma/retired``` | Returns the list of inactive FISMA Systems

| ```/investments``` | Returns the complete list of GSA's IT Investments, as tracked in GEAR
| ```/investments/get/{id}``` | Returns one IT Investment identified by {id}
| ```/investments/get/{id}/applications``` | Returns the Business Applications that are related to the IT Investment identified by {id}
| ```/investments/latest``` | Returns the most recently created Investment item
| ```/investments/types``` | Returns the list of possible investment types

| ```/itstandards``` | Returns the entire list of GSA's Software IT Standards 
| ```/itstandards/get/{id}``` | Returns one IT Standard identified by {id}
| ```/itstandards/get/{id}/applications``` | Returns the Business Applications and Business Application metadata associated to the indicated IT Standard {id}
| ```/itstandards/latest``` | Returns the most recently created IT standard item
| ```/itstandards/508_compliance``` | Returns the list of possible 508 Compliance statuses
| ```/itstandards/categories``` | Returns the list of possible IT standards categories
| ```/itstandards/deployment_types``` | Returns the list of possible IT standards deployment types
| ```/itstandards/statuses``` | Returns the list of possible IT standards statuses
| ```/itstandards/types``` | Returns the list of possible IT standards types

| ```/organizations``` | Returns the complete list of GSA's Organizations, as they are tracked in GEAR
| ```/organizations/get/{id}``` | Returns one Organization identified by {id}
| ```/organizations/get/{id}/applications``` | Returns the Business Applications that are related to the Organization identified by {id}

| ```/parentsystems``` | Returns the complete list of GSA's Parent Systems
| ```/parentsystems/get/{id}``` | Returns one System identified by {id}
| ```/parentsystems/get/{id}/applications``` | Returns the Child Business Applications that make up the System identified by {id}
| ```/parentsystems/latest``` | Returns the most recently created Parent System item

| ```/pocs``` | Returns the list of all POCs tracked in GEAR
| ```/pocs/get/{id}``` | Returns one POC identified by {id}
| ```/pocs/risso``` | Returns RISSO indicated POCs and associated metadata

| ```/search/{kw}``` | Returns a list of applications, capabilities, FISMA systems, investments, IT Standards, and Parent Systems that match or contains the term {kw}

<body id="basics"></body>
