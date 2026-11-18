Using API Calls Page (/console)
====================

This readme explains some of the intricacies of using the API Calls page, which is in the /console directory of this project. (Some of these intricacies could be improved by future updates.)

## Navigation Bar
The API Calls page has a hard-coded version of the navigation bar that matches the rest of the site.

You can find it in the /console/index.html file by searching for class="page-title". Notice that the relative path of the links are different in this page than in the master nave bar (which is in the _includes).


## Swagger Container
The Swagger UI container is injected into the DOM by JavaScript. If you are looking at the output HTML, you will see that it begins with this tag: 

```
<div id="swagger-ui-container" class="swagger-ui-wrap"> 
```

The actual contents of the Swagger UI container are generated from the Swagger 2.0 specification at `/console/gear.json`. The console loads this file by default; `citypairs.json` is a separate sample specification. This repository documents APIs but does not implement their server-side behavior.

## Adding an API operation

Add each operation to the `paths` object in `gear.json`. The specification already sets `basePath` to `/api`, so path keys should omit that prefix. For example, document `GET /api/tech_catalog/get/manufacturers` under `/tech_catalog/get/manufacturers`.

For each operation, include its HTTP method, tag, summary, description, parameters, and success response schema. Add or reuse a definition under `definitions` for request bodies and response data. Document authentication only when it is specified by the route contract; never write a real API token into this repository.

The current GEAR specification is read-only and intentionally omits POST and PUT operations. The supplied API contract identifies `/dashboard_summary` and `/dashboard_summary/hosting_platforms` as the dashboard routes; follow the individual route declarations when documenting paths and methods.

The Swagger specification can be edited or checked with [Swagger Editor](https://editor.swagger.io/). Confirm that the updated `gear.json` parses and that the operation appears in the console.
