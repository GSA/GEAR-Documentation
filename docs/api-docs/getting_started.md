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
| ------------- | -------------|
| ```version 0``` | *Look this up* | Initial deployment using node.js and Express


#### Endpoints

| Endpoint | What it does |
| ------------- | -------------|
| ```/applications/``` | Returns the complete list of GSA Business Applications, to include retired applications 
| ```/applications/{id}``` | Returns one Business Application by {id}
| ```/itstandards/``` | Returns the entire list of GSA's Software IT Standards 
| ```/itstandards/{id}``` | Returns one IT Standard by {id}


<body id="basics"></body>
