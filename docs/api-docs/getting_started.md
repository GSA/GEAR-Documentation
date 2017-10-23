---
layout: default
title: API Basics
nav: basics
---

### Getting Started

The current version of the API lives at ```https://ea.gsa.gov/api/v0/...```

- These endpoints each return a list of objects, or can be limited to a particular {id}.
- Some endpoints have further attributes that bring back other objects related to that {id}. 
- A [Glossary of GEAR terms](https://ea.gsa.gov/#!/glossary) can help define some of these objects. 

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
| ```/applications/{id}/technologies``` | Returns the IT Technologies and IT Technologies metadata associated to the indicated Business Application {id}
| ```/applications/{id}/pocs``` | Returns the POCs related to the indicated Business Application {id}
| ```/applications/{id}/interfaces``` | Returns one Business Application by {id}
| ```/itstandards/``` | Returns the entire list of GSA's Software IT Standards 
| ```/itstandards/{id}``` | Returns the Interfaces related to the indicated Business Application {id}


<body id="basics"></body>
