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
| ```version 2``` | 08/01/2023 | Updates and rewrite of entire GEAR platform
| ```version 1``` | 09/25/2020 | Updates and rewrite of entire GEAR platform
| ```version 0``` | 03/31/2017 | Initial deployment using node.js and Express

<!-- 
#### Endpoints

| Endpoint | What it does |
| ------------- | -------------|
| ```/systems``` | Returns the complete list of GSA Business Systems, to include retired applications
| ```/systems/get/{id}``` | Returns one Business System by {id}
| ```/systems/get/{id}/capabilities``` | Returns the Business Capabilites and Business Capability metadata associated to the indicated Business System {id}
| ```/systems/get/{id}/technologies``` | Returns the IT Standards and IT Standards metadata associated to the indicated Business System {id}
| ```/systems/systems_retired``` | Returns the list of all retired GSA Business Systems
| ```/systems/latest``` | Returns the most recently created GSA Business System
| ```/systems/statuses``` | Returns the list of possible system statuses
| ```/systems/host_providers``` | Returns the list of possible host providers for GSA Business Systems

| ```/system_time``` | Returns all entries for TIME analysis of all Active GSA Business Systems
| ```/system_time/get/{id}``` | Returns all entries for TIME analysis of the indicated Business System {id}

| ```/capabilities``` | Returns the complete list of GSA's Business Capabilities
| ```/capabilities/{id}``` | Returns one Business Capability indecated by {id}
| ```/capabilities/{id}/systems``` | Returns the Business Systems that are related to the Business Capability identified by {id}
| ```/capabilities/sso/{name}``` | Returns the Business Capabilities that are related to the SSO organization identified by {name}

| ```/data_flow``` | Returns the complete lit of data flow entries for all GSA Business Systems
| ```/data_flow/get/{id}``` | Returns the Business Systems that interface with the Business System identified by {id}

| ```/fisma``` | Returns the list of GSA's FISMA Systems, excluding inactive systems
| ```/fisma/{id}``` | Returns one FISMA System identified by {id}
| ```/fisma/{id}/systems``` | Returns the Business Systems and Business System metadata associated to the indicated FISMA System {id}
| ```/fisma/retired``` | Returns the list of inactive FISMA Systems

| ```/investments``` | Returns the complete list of GSA's IT Investments, as tracked in GEAR
| ```/investments/get/{id}``` | Returns one IT Investment identified by {id}
| ```/investments/get/{id}/systems``` | Returns the Business Systems that are related to the IT Investment identified by {id}
| ```/investments/latest``` | Returns the most recently created Investment item
| ```/investments/types``` | Returns the list of possible investment types

| ```/itstandards``` | Returns the entire list of GSA's Software IT Standards 
| ```/itstandards/get/{id}``` | Returns one IT Standard identified by {id}
| ```/itstandards/get/{id}/systems``` | Returns the Business Systems and Business System metadata associated to the indicated IT Standard {id}
| ```/itstandards/latest``` | Returns the most recently created IT standard item
| ```/itstandards/508_compliance``` | Returns the list of possible 508 Compliance statuses
| ```/itstandards/categories``` | Returns the list of possible IT standards categories
| ```/itstandards/deployment_types``` | Returns the list of possible IT standards deployment types
| ```/itstandards/statuses``` | Returns the list of possible IT standards statuses
| ```/itstandards/types``` | Returns the list of possible IT standards types

| ```/organizations``` | Returns the complete list of GSA's Organizations, as they are tracked in GEAR
| ```/organizations/get/{id}``` | Returns one Organization identified by {id}
| ```/organizations/get/{id}/systems``` | Returns the Business Systems that are related to the Organization identified by {id}

| ```/parentsystems``` | Returns the complete list of GSA's Parent Systems
| ```/parentsystems/get/{id}``` | Returns one System identified by {id}
| ```/parentsystems/get/{id}/applications``` | Returns the Child Business Applications that make up the System identified by {id}
| ```/parentsystems/latest``` | Returns the most recently created Parent System item

| ```/pocs``` | Returns the list of all POCs tracked in GEAR
| ```/pocs/get/{id}``` | Returns one POC identified by {id}
| ```/pocs/risso``` | Returns RISSO indicated POCs and associated metadata

| ```/search/{kw}``` | Returns a list of applications, capabilities, FISMA systems, investments, IT Standards, and Parent Systems that match or contains the term {kw} -->

<body id="basics"></body>
