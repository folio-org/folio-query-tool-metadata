# folio-query-tool-metadata
Copyright (C) 2023 The Open Library Foundation

This software is distributed under the terms of the Apache License,
Version 2.0. See the file "[LICENSE](LICENSE)" for more information.

## Introduction
folio-query-tool-metadata is responsible for defining the API for the mod-fqm-manager and edge-fqm modules,
including the object models that are part of that API.

## Building
```bash
mvn clean install
```

# Usage
Simply add this library as a dependency to a module:
```xml
<dependency>
    <group>org.folio</group>
    <artifactId>folio-query-tool-metadata</artifactId>
    <version>1.0.0</version>
</dependency>
```

Then, implement the `EntityTypesApi` and `FqlQueryApi` interfaces.

## Additional information

### Issue tracker

See project [FQTM](https://issues.folio.org/browse/FQTM)
at the [FOLIO issue tracker](https://dev.folio.org/guidelines/issue-tracker).

### Code of Conduct

Refer to the Wiki
[FOLIO Code of Conduct](https://wiki.folio.org/display/COMMUNITY/FOLIO+Code+of+Conduct).

### API documentation

API descriptions:

* [OpenAPI](src/main/resources/swagger.api/queryTool.yaml)
* [Schemas](src/main/resources/swagger.api/schemas/)

Generated [API documentation](https://dev.folio.org/reference/api/#folio-query-tool-metadata)

### Code analysis

[SonarQube analysis](https://sonarcloud.io/project/overview?id=org.folio%3Afolio-query-tool-metadata).

### Download and configuration

The built artifacts for this module are available.
See [configuration](https://dev.folio.org/download/artifacts) for repository access
