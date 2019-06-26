![Custom Shield](https://img.shields.io/badge/updatedAt-2019/06/25-green.svg?style=for-the-badge) ![Custom Shield](https://img.shields.io/badge/type-MARKDOWN_NOTE-blue.svg?style=for-the-badge) ![Custom Shield](https://img.shields.io/badge/folder-4bfaf976594ec1b5be18-blue.svg?style=for-the-badge) ![Custom Shield](https://img.shields.io/badge/tag-Random_Tag-purple.svg?style=for-the-badge) ![Custom Shield](https://img.shields.io/badge/tag-Taggy_Bear-purple.svg?style=for-the-badge) ![Custom Shield](https://img.shields.io/badge/tag-TODOs-purple.svg?style=for-the-badge)
# Day: Tuesday  Date: June 18
# 📑TODOS:
- [ ] Give an option where in people can fall back to default behaviour if any value gives an error.
- [x] Add interactive mode.
- [x] Change config to Dict.
- [x] Adding YAML support.
- [x] Ask only few options in CLI mode.
- [ ] Format All the variables in templates.
- [ ] Set the emojis.
- [ ] Convert all the template files to write functions.
  - [x] Make ReadMe.
  - [x] Make Licences.
    - [x] MIT
    - [x] unilicense
    - [x] agpl-3.0
    - [x] apache-2.0
    - [x] GNU2
    - [x] GNU GPLv3
    - [x] gpl-3.0
    - [x] lgpl-3.0
    - [x] mpl-2.0
  - [x] Make Dockerfile.
  - [x] Make Manifest.ini
  - [ ] Make SCRIPT.SH to make everything ez.
  - [ ] Make .codeclimate.yml
  - [ ] MAke .codecoveragerc
  - [x] MAke isort/black config.
  - [ ] Make CIs
    - [ ] Appveyor
    - [ ] Tox
    - [ ] Travis
    - [ ] Make test
      - [ ] Add __init__.py
  - [ ] Make .gitignore

----
# Sample Yaml Settings:

``````
project_name: 'PrjectGetGPA'
project_version: 0.01alpha
project_description: 'Working project has the following descriptions. I dont even remember                                       how to write fast of this things. I have gotten so function slow.'
author_name: 'Ratin Kumar'
github_username: 'DumbMachine'

**If Default is True, all below options will be ignored.**
default: False

license: 'MIT'
git: True 
colour: True
interactive: False

files:
  setup_py: True
  setup_cfg: True
  main: True
  manifest: False
  setup.cfg: False
  docker: False
  requirements: True
  contributing: True
  readme: 'markdown'

shields:
  build: 'appveyor'
  codecov: 'codecov'
  analysis: 'gtihub-lanugage-count'
  chat: 'discord'
  dependencies:
  size: 'github-repo-size'
  downloads:
  funding:
  issues:
  license: 'github'
  rating:
  social:
  version: 'pypi'
  platform:
  monitoring:
  activity:
  other:
``````