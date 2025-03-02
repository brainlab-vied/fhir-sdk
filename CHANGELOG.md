# Changelog

All notable changes to this project will be documented in this file.

## [0.6.0] - 2023-09-16

### Bug Fixes

- Do not filter out codes like HTTPVerb
- Go deeper into the codes, there are more layers

### Features

- Implement batch/transaction requests
- Implement Encounter $everything operation
- Implement Patient $everything and $match
- Implement PATCH

### Refactor

- Change the way references are parsed

### Testing

- Refactor to use batches

## [0.5.0] - 2023-09-08

### Bug Fixes

- Have the doc-test only at the right features
- Impl Send for returned Stream
- Base64 needs to use padding and strip whitespaces

### Documentation

- Add search to example

### Features

- Implement creation of References
- Add Reference parsing
- Implement reading a referenced resource
- Add getters for code by system for CodeableConcept
- Implement Rust types for primitive FHIR types
- Generate models using new primitive types

### Miscellaneous Tasks

- Update generator fhir-model

### Performance

- Use optimized proc macro compilation

### Refactor

- Move misc functions to module
- Move and rename reference creation methods

### Testing

- Create xtask test command
- Reference search
- Fetch referenced resource
- Adjust to new primitive date types
- Adjust JSON comparison to FHIR to fix tests

## [0.4.1] - 2023-09-01

### Bug Fixes

- Make everything compile with different features

### Features

- Add back search for all resources
- Allow to disable builders
- Implement getting the server's capabilities

### Miscellaneous Tasks

- Improve README

### Testing

- Use local test server

## [0.4.0] - 2023-08-31

### Bug Fixes

- Improve code generation using cleaner URL usage
- Do not override headers with default headers
- Adjust wrong LinkRelationTypes definitions
- Implement Copy for ResourceType
- Implement Display for ResourceType

### Documentation

- Improve generated doc comments

### Features

- Implement basic REST client
- Implement paging
- Implement search with typed helpers

### Miscellaneous Tasks

- Fix new clippy lints
- Add expansions for R4B and remove unneeded definitions
- Update typed-builder and fhir-sdk dependencies
- Update README

## [0.3.0] - 2023-04-01

### Bug Fixes

- Integer64 is actually a JSON String
- Add values for RelatedArtifactTypeExpanded
- [**breaking**] Choice field extensions include the value type in the field name
- Specimen.combined actually links to SpecimenCombined, not PublicationStatus

### Features

- Add FHIR R5 files
- Generate R5 models

### Refactor

- Use own FHIR models for code generation

## [0.2.0] - 2023-03-26

### Features

- Implement code conversion to Coding and CodeableConcept
- Implement base traits for all resources
- Implement IdentifiableResource
- Extend the IdentifiableResource trait

### Miscellaneous Tasks

- Add resolver = 2

## [0.1.0] - 2023-03-24

### Features

- Initial implementation

<!-- generated by git-cliff -->
