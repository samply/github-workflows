# Change Log
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/)
and this project adheres to [Semantic Versioning](http://semver.org/).

## [1.0.5 - 2022-05-31]
### Fixed
- Added if condition for steps regarding docker hub, so that they aren't run on pull requests

## [1.0.4 - 2022-05-31]
### Changed
- Removed automated addition of - from to the prefix. This led to errors then no prefix was added. If users supply a prefix, they're free to add the minus themselves.

## [1.0.3 - 2022-05-31]
### Fixed
- Removed build-args input, because list type is currently not supported by github actions.

## [1.0.2 - 2022-05-31]
### Fixed
- Added secret declaration for docker-ci action

## [1.0.1 - 2022-05-31]
### Fixed
- Added runs-on definition for docker-ci action

## [1.0.0 - 2021-12-21]
### Added
- Workflow for Building, Testing and Publishing Maven Packages [maven.yml](./github/workflows/maven.yml)
- Workflow for Building and Publishing a Docker Image [docker-ci.yml](./github/workflows/docker-ci.yml)
