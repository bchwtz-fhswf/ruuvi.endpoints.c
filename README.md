# ruuvi.endpoints.c
Data endpoints for abstracting source (e.g. bme280) from data (e.g. temperature).

![GH-Pages](https://github.com/ruuvi/ruuvi.endpoints.c/workflows/GH-Pages/badge.svg)
![Ceedling](https://github.com/ruuvi/ruuvi.endpoints.c/workflows/Ceedling/badge.svg)
![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=ruuvi.endpoints.c&metric=alert_status)
![Coverage](https://sonarcloud.io/api/project_badges/measure?project=ruuvi.endpoints.c&metric=coverage)
![Bugs](https://sonarcloud.io/api/project_badges/measure?project=ruuvi.endpoints.c&metric=bugs)
![Code Smells](https://sonarcloud.io/api/project_badges/measure?project=ruuvi.endpoints.c&metric=code_smells)

# Embedding to your application
Include a tagged release to your application as a git submodule.
If you define `APPLICATION_ENDPOINTS_CONFIGURED` in preprocessor, you can select which endpoints to compile by adding
definitions `#define RE_3_ENABLED 1` , `#define RE_5_ENABLED 1`  etc in "app_config.h" inside your application.

# Developing
## Unit testing
Unit tests are run by Ceedling.

## Static code analysis
Test coverage and code analysis are reported by [Sonarcloud](https://sonarcloud.io/dashboard?id=ruuvi.endpoints.c). Additionally the project is analyzed with PVS Studio and report is published to [GH Pages](https://ruuvi.github.io/ruuvi.endpoints.c/fullhtml)

## Styling
Styling is done via Artisitic Style, following configuration at .astylerc. 

## Documentation
Documentation is autogenerated to [GH-Pages](https://ruuvi.github.io/ruuvi.endpoints.c/).
On pull requests, the documentation is generated to gh-pages-check branch.

# Changelog

## 3.0.1 Fix CA UART Get ID command
 - Used to send ID twice instead of ID + ADDR

## 3.0.0 Initial release