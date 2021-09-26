# Codedigger Backend API

[![Codedigger][codedigger-shield]][Codedigger]
[![Codedigger API][codedigger-api-shield]][API]
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![Apache License][license-shield]][license-url]
[![Contributor Covenant][code-of-conduct-shield]][code-of-conduct-url]
[![PRs Welcome][pr-shield]][makeapullrequest]
[![LinkedIn][linkedin-shield]][linkedin-url]
[![Discord][discord-shield]][discord-url]

## Table of Contents

1. [Introduction](#introduction)
1. [Getting Started](#getting-started)
1. [Contributing](#contributing)
1. [License](#license)
1. [How to Get Help](#how-to-get-help)


## Introduction

This is the backdoor REST [API] developed to do complex calclations, provide and store data for [Codedigger] Website. 

Codedigger aims at accumulating the data of competitive programming platforms ([Codeforces], [Codechef], [Atcoder], [SPOJ] and [UVA Online Judge]) into one platform. We used their publicly available APIs and introduced several unique features into our application such as friends, mentors, ladders, upsolve, problem and contest filter. This can be the ultimate stop for everyone practicing competitive programming.

User can practice topicwise list to expertise any topic, levelwise list to practice based on rating and difficulty, or can create their own list and follow that. They can filter problems based on difficulty, tag, or solved by mentor from all the sites combined at one place.

Upsolving means to solve those problems, you're not able to solve during the contest. With the help of codedigger, you will be able to upsolve codeforces, codechef, and atcoder contests in an easy and better way.


## Getting Started

#### Setting Environment First Time
Below commands will setup the environment for the first time.

#### Windows
```
py -m pip install --user virtualenv
py -m venv env
```
#### Linux
```
python3 -m pip install --user virtualenv
python3 -m venv env
```

### This project uses MySQL database , first you have to setup MySQL database. 
```
Download XAMPP from [here](https://www.apachefriends.org/download.html)
Start MySQL server.
```

#### Starting Virtual Env. and Setting up the Project
Below are the commands for project Initialization into your local computer
#### For Windows
```
. env/Scripts/activate -- If using gitbash
. env\Scripts\activate -- If using Windows Powershell
pip install -r requirements.txt
cd codedigger
py manage.py migrate
py manage.py runserver
```
- This would start the development server

#### For Linux
```
source env/bin/activate
pip3 install -r requirements.txt
cd codedigger
python3 manage.py migrate
python3 manage.py runserver
```
- This would start the development server 

### Leaving the virtual environment
```
deactivate
```

### To update requirements file 
```
pip freeze > requirements.txt
```

## Contributing

We encourage public contributions! Please review [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct and development process.

<!-- LICENSE -->
## License

Copyright 2021 Codedigger

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

	http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.


<!-- CONTACT -->
## How to Get Help 

Email us - contact.codedigger@gmail.com

[Join][discord-url]! our Discord Community

**[Back to top](#table-of-contents)**


<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/Code-dig-ger/Backend.svg?style=for-the-badge
[contributors-url]: https://github.com/Code-dig-ger/Backend/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/Code-dig-ger/Backend.svg?style=for-the-badge
[forks-url]: https://github.com/Code-dig-ger/Backend/network/members
[stars-shield]: https://img.shields.io/github/stars/Code-dig-ger/Backend.svg?style=for-the-badge
[stars-url]: https://github.com/Code-dig-ger/Backend/stargazers
[issues-shield]: https://img.shields.io/github/issues/Code-dig-ger/Backend.svg?style=for-the-badge
[issues-url]: https://github.com/Code-dig-ger/Backend/issues
[license-shield]: https://img.shields.io/github/license/Code-dig-ger/Backend.svg?style=for-the-badge
[license-url]: https://github.com/Code-dig-ger/Backend/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/company/codedigger
[code-of-conduct-shield]: https://img.shields.io/badge/Contributor%20Covenant-2.0-4baaaa.svg
[code-of-conduct-url]: CODE_OF_CONDUCT.md
[pr-shield]: https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square
[makeapullrequest]: http://makeapullrequest.com
[discord-shield]: https://img.shields.io/badge/Discord--555?style=for-the-badge&logo=discord&logoColor=white
[discord-url]: https://discord.gg/4ZeNgUn7cF
[API]: https://api.codedigger.tech/
[Codedigger]: https://codedigger.tech
[Codeforces]: https://codeforces.com/
[Codechef]: https://www.codechef.com/
[Atcoder]: https://atcoder.jp/
[SPOJ]: https://www.spoj.com/
[UVA Online Judge]: https://onlinejudge.org/
[codedigger-shield]: https://img.shields.io/badge/Codedigger--555?style=for-the-badge&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABQAAAAUCAYAAACNiR0NAAAAAXNSR0IArs4c6QAAAuFJREFUOE+t1G1IE3EcB/DvFEPnmDrN5sPKxKGixgqns5n0oiezMl8EQSgESW8SqiFBRdCLMEhCKyopyNIsDErrRdmDmrFUlKInsGTMBW63ebc5t91s3ba43c5tmCHkwb24O/jc9////f4/AVb4Eqywh6VBoTANwoRqMIwStD2jsOUcflM2o/3zxNjcwGgvTZLGv4VZDIpEqShQNyFeVAuSiAFlAigC6lf3ECWIgtdFg3HSzMy74fv6ru5TsLjM4XAkKMstxo4Dz+Cck4I0YeG2BkEAjMsNr8sNxkXDQ9rMuuvt1e7JqVEeDYGrM+U4cnYUDlsSSCKEsbCVQPnrDgh8vgjQS9PwWO123dVbKo+RmmDREHiydQjixC1cKgLsUqPsFmSW50OiyEVCgRw+N5sslJAFvU4ajh/6EUNb52YAfg7MV1bg2IW3oWQEoh0z2NRQhST5WvgYJrDEwP6FgwvvaEzdfrht/uf0Gw48pGmGepcmHFyvkkG+pyTweTHIw9xP2D219GtbqcHh4xx4ovkp5Iq9bDX5QhQfVkOSLf0HyEE8aPvw5TnR07ebAzUtvcgp2sclNAKUGcV1pZDkpC8TpDH78esL05O+Sg6sbWyGulITahUC6zZKkVtTtmzQ0v/+GjU43MCBhaqtaGgaWEhIEoiaNUNRvx0phdlL7GFoyWzB9Hce7PylN77k20aA021axIvLAicj2IcCqxlShQzJRdmQKDfA7/EEqxxZFMfk1LjhZgdbwWDbsCnTs/JQf34EDmtCeHH4bVA9uoIYYWywffh+pOGx2R261vYyD0F8i2xs9ikrX4Wqul447akBKJCWu0u7LmOVOJ4DnW4w7CmhbKThRud+x3eddvHR498IU9JQUnEJIvFBkKZoHla2X0RsciI7GFjUS2nHu013Hze6KWp66eEQ/iUuToakNTXw+pWg5zLyzhz1w+czOT9NjJFDYz3zJpNheePrPyfuik/sP0+iITNZPL3cAAAAAElFTkSuQmCC
[codedigger-api-shield]: https://img.shields.io/badge/Codedigger-API-yellowgreen?style=for-the-badge&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABQAAAAUCAYAAACNiR0NAAAAAXNSR0IArs4c6QAAAuFJREFUOE+t1G1IE3EcB/DvFEPnmDrN5sPKxKGixgqns5n0oiezMl8EQSgESW8SqiFBRdCLMEhCKyopyNIsDErrRdmDmrFUlKInsGTMBW63ebc5t91s3ba43c5tmCHkwb24O/jc9////f4/AVb4Eqywh6VBoTANwoRqMIwStD2jsOUcflM2o/3zxNjcwGgvTZLGv4VZDIpEqShQNyFeVAuSiAFlAigC6lf3ECWIgtdFg3HSzMy74fv6ru5TsLjM4XAkKMstxo4Dz+Cck4I0YeG2BkEAjMsNr8sNxkXDQ9rMuuvt1e7JqVEeDYGrM+U4cnYUDlsSSCKEsbCVQPnrDgh8vgjQS9PwWO123dVbKo+RmmDREHiydQjixC1cKgLsUqPsFmSW50OiyEVCgRw+N5sslJAFvU4ajh/6EUNb52YAfg7MV1bg2IW3oWQEoh0z2NRQhST5WvgYJrDEwP6FgwvvaEzdfrht/uf0Gw48pGmGepcmHFyvkkG+pyTweTHIw9xP2D219GtbqcHh4xx4ovkp5Iq9bDX5QhQfVkOSLf0HyEE8aPvw5TnR07ebAzUtvcgp2sclNAKUGcV1pZDkpC8TpDH78esL05O+Sg6sbWyGulITahUC6zZKkVtTtmzQ0v/+GjU43MCBhaqtaGgaWEhIEoiaNUNRvx0phdlL7GFoyWzB9Hce7PylN77k20aA021axIvLAicj2IcCqxlShQzJRdmQKDfA7/EEqxxZFMfk1LjhZgdbwWDbsCnTs/JQf34EDmtCeHH4bVA9uoIYYWywffh+pOGx2R261vYyD0F8i2xs9ikrX4Wqul447akBKJCWu0u7LmOVOJ4DnW4w7CmhbKThRud+x3eddvHR498IU9JQUnEJIvFBkKZoHla2X0RsciI7GFjUS2nHu013Hze6KWp66eEQ/iUuToakNTXw+pWg5zLyzhz1w+czOT9NjJFDYz3zJpNheePrPyfuik/sP0+iITNZPL3cAAAAAElFTkSuQmCC