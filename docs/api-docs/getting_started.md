---
layout: default
title: API Basics
nav: basics
---

### Getting Started

The current version of the API lives at ```https://ea.gsa.gov/api/v0/...```

- These endpoints each return a list of objects, or can be limited to a particular {id}.
- Some endpoints have further attributes that bring back other objects related to that {id}. 
- A [Glossary of GEAR terms](https://ea.gsa.gov/#!/glossary) can help define some of these objects. (You will need to be on the GSA network to reach the glossary) 

#### Versions

| Version | Date | Changes | 
| ------------- | ------------- | ------------- |
| ```version 0``` | 03/31/2017 | Initial deployment using node.js and Express


#### Endpoints

| Endpoint | What it does |
| ------------- | -------------|
| ```/applications/``` | Returns the complete list of GSA Business Applications, to include retired applications 
| ```/applications/{id}``` | Returns one Business Application by {id}
| ```/applications/{id}/capabilities``` | Returns the Business Capabilites and Business Capability metadata associated to the indicated Business Application {id}
| ```/applications/{id}/technologies``` | Returns the IT Standards and IT Standards metadata associated to the indicated Business Application {id}
| ```/applications/{id}/pocs``` | Returns the POCs related to the indicated Business Application {id}
| ```/applications/{id}/interfaces``` | Returns the Business Applications that interface with the Business Application identified by {id}
| ```/itstandards/``` | Returns the entire list of GSA's Software IT Standards 
| ```/itstandards/{id}``` | Returns one IT Standard by {id}
| ```/itstandards/{id}/applications``` | Returns the Business Applications and Business Application metadata associated to the indicated IT Standard {id}
| ```/fisma``` | Returns the complete list of GSA's FISMA Systems
| ```/fisma/{id}``` | Returns one FISMA System by {id}
| ```/fisma/{id}/applications``` | Returns the Business Applications and Business Application metadata associated to the indicated FISMA System {id}
| ```/fisma/pocs``` | Returns POCs and metadata for all FISMA Systems
| ```/fisma/{id}/pocs``` | Returns POCs and metadata associated to the indicated FISMA System {id}
| ```/pocs``` | Returns RISSOs and associated metadata
| ```/parentsystems``` | Returns the complete list of GSA's Systems
| ```/parentsystems/{id}``` | Returns one System by {id}
| ```/parentsystems/{id}/applications``` | Returns the Business Applications that make up the System identified by {id}
| ```/organizations``` | Returns the complete list of GSA's Organizations, as they are tracked in GEAR
| ```/organizations/{id}``` | Returns one Organization by {id}
| ```/organizations/{id}/applications``` | Returns the Business Applications that are related to the Organization identified by {id}
| ```/capabilities``` | Returns the complete list of GSA's Business Capabilities
| ```/capabilities/{id}``` | Returns one Business Capability by {id}
| ```/capabilities/{id}/applications``` | Returns the Business Applications that are related to the Business Capability identified by {id}
| ```/investments``` | Returns the complete list of GSA's IT Investments, as tracked in GEAR
| ```/investments/{id}``` | Returns one IT Investment by {id}
| ```/investments/{id}/applications``` | Returns the Business Applications that are related to the IT Investment identified by {id}
| ```/investments/{id}/poc``` | Returns the details for the Investment Manager that is related to the IT Investment identified by {id}




<body id="basics"></body>
