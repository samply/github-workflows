# Change Log
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/)
and this project adheres to [Semantic Versioning](http://semver.org/).

## [1.3.2 - 2022-07-21]
### Fixed
- latest tag should now be created automatically on default branch, as intended
## [1.3.1 - 2022-07-21]
### Changed
- Switched to new Trivy Syntax for exporting sarif security scan results
## [1.3.0 - 2022-07-19]
### Added
- Added Syntax to Download all Artifacts from a Pipeline
## [1.2.1 - 2022-07-18]
### Changed
- Security Scan for Images will now ignore unfixable issues
## [1.2.0 - 2022-07-15]
### Added
- Documentation in docker-ci.yml
### Changed
- To avoid name collisions, artifacts are -- by convention, not configuration -- always downloaded into directory ./artifacts/
- Updated to actions/download-artifact@v3

## [1.1.1 - 2022-06-02]
### Fixed
- Removed platform specification from first Docker Build, due to conflicts with the load option

## [1.1.0 - 2022-06-01]
### Added
- Added input for changing the target platforms of the docker build.

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
