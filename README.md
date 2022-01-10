# Talk Liberation Investigates [GETTR](https://talkliberation.com/gettr)
https://talkliberation.com/gettr

## Introduction

[This repository](https://talkliberation.com/gettr-repo) contains supporting material for an investigation by [Talk Liberation](https://talkliberation.substack.com) into the [GETTR](https://en.wikipedia.org/wiki/Gettr) social media platform and smartphone apps conducted in January 2022.

All of these files were obtained via technical analyis with freely-available and Free and Open-Source Software (FOSS) tools, and none of the published information was obtained via leaks, hacking, or data breaches.

Talk Liberation encourages readers to independently validate this work and to develop it further. The information here is provided for context as well as journalistic and technical exploration beyond the scope of our initial investigation.

## Key Findings
* Numerous trackers from Facebook, Google, and other third parties are embedded in GETTR web and smartphone apps.

* App permissions facilitate the surveillance of a wide variety of information about GETTR users, including fine-grained behavior and location data. This data is then used to profile users and shared with third parties.

* “Getome,” a previous version of the GETTR app that targeted Chinese-language audiences, is still published in Google Play and effectively provides a backdoor to GETTR. Users can log in and interact on the GETTR network via the Getome app, bypassing updates on the newer application.

* Content on GETTR such as news is loaded directly from external sources, opening connections between GETTR users to dozens of domains. This introduces serious privacy and security risks. Some of this content is delivered via unencrypted HTTP, further jeopardizing users.

* GETTR’s privacy policies fail to disclose the full extent of GETTR data collection and sharing with third parties.

* GETTR infrastructure is hosted by cloud vendors such as Amazon AWS and company email accounts are hosted by Google.

* Utilizing the API of GETTR to gather large amounts of data is trivial. The situation has improved since approx. 90,000 emails were breached in July 2021, but a trove of information is still available via basic technical methods.

[Read Our Detailed Analysis...](https://talkliberation.com/gettr)

## Table of Contents

A listing of directories in this repository and a short description of the files within is available below.

### [Smartphone App Analysis](smartphone)
These files relate to static analysis, dynamic analysis, and network analysis of the GETTR and Getome smartphone apps, including privacy and security information such as call graphs derived from code.

### [Web App Analysis](web)
These files relate to static analysis, dynamic analysis, and network analysis of the GETTR web app at _gettr.com_, including privacy and security information such as JSON output from the GETTR API.

## Licensing

Any and all original work contained in this repository that is authored by Sean O'Brien for Talk Liberation is released under the [CC0 Public Domain Dedication](https://creativecommons.org/publicdomain/zero/1.0/) and the author has waived all copyright and related or neighboring rights to that work, to the extent possible under law.

The articles written on [talkliberation.substack.com](https://talkliberation.substack.com) are © Copyright Talk Liberation CIC Limited and licensed under a [Creative Commons Attribution-ShareAlike 4.0 International](https://creativecommons.org/licenses/by-sa/4.0/) license. Contact Talk Liberation for further information or additional permissions.

## Contact

For media inquiries, please contact [media@talkliberation.com](mailto:media@talkliberation.com)

