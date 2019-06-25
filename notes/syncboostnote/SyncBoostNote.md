![Custom Shield](https://img.shields.io/badge/updatedAt-2019/06/25-green.svg?style=for-the-badge) ![Custom Shield](https://img.shields.io/badge/type-MARKDOWN_NOTE-blue.svg?style=for-the-badge) ![Custom Shield](https://img.shields.io/badge/folder-4bfaf976594ec1b5be18-blue.svg?style=for-the-badge) ![Custom Shield](https://img.shields.io/badge/tag-Taggy_Bear-purple.svg?style=for-the-badge) ![Custom Shield](https://img.shields.io/badge/tag-Documentation-purple.svg?style=for-the-badge) ![Custom Shield](https://img.shields.io/badge/tag-Breathtaking-purple.svg?style=for-the-badge) ![Custom Shield](https://img.shields.io/badge/tag-👌-purple.svg?style=for-the-badge)
# SyncBoostNote
[![forthebadge](https://forthebadge.com/images/badges/built-with-love.svg)](https://forthebadge.com)  [![forthebadge](https://forthebadge.com/images/badges/made-with-python.svg)](https://forthebadge.com)
[![forthebadge](https://img.shields.io/badge/Made%20For-Boostnote-brightgreen.svg?style=for-the-badge)](https://github.com/BoostIO/Boostnote) [![forthebadge](https://img.shields.io/badge/STATUS-WIP-blueviolet.svg?style=for-the-badge)](https://github.com/BoostIO/Boostnote) 


### A simple cli to save your notes from Boostnotes directly to a Github repo.

## Features:


## Requirements:
### Before using this cli, make sure you have the following:
- git
  - If not installed visit, [Git](https://git-scm.com/downloads)
- python
- boostnote (also know where it is installed)
  - If not installed visit, [BoostNote](https://boostnote.io/#download)
## Installation:
- To install from PyPi:
```bash
$ pip install syncboostnote
```
- To install from source:
```bash
$ git clone https://github.com/DumbMachine/SyncBoostNote
$ cd syncboostnote
$ python setup.py install
```
## Usage:
### Default Usage:
This method assumes that the location of ``Boostnote`` local storage is the following:
```bash
/home/$USER/Boostnote
```
If this indeed is the location of the installation, then you don't really have to do anything.
1. Create a Repo on github ( or use an existing one ), where you would like notes to be saved.
2. Go to installation directory:
```bash
$ cd ~/Boostnote
```
3. Initialise a git repository and add the remote to your desired repository.
```bash
$ git init
$ git remote add origin <repo_url>
```
4. Let the cli take control now. Since your already have the correct location for ``Boostnote`` folder, all you have to do now is:
```bash
$ syncboostnote  # This will call the cli
```
This will add all your notes to repo and also generate ``.md`` files for them. ( placed in the */Boostnote/note/syncboostnote ). 
5. To publish the added notes to your github repo
```bash
$ syncboostnote --sync
```
This will upload the folder ``Boostnote`` to github with the following tree:
```bash
$ tree Boostnote
Boosnote
├── boostnote.json
├── history.json
├── notes
|    ├── ....cson
|    ├── ....cson
|    └── syncboostnote
|        ├── ....md
|        ├── ....md
├──── README.md

```
- Directory `boostnote`:
  - boostnote.json ``Created by boostnote``
  - history.json ``Created by SyncBoostnote``
  - Directory `notes`:
    - Raw `.cson` files used by BoostNote.
    - Directory `syncboostnote`:
      - `.md` files used display content on Github.
  - ``README.md`` Created by ``SyncBoostnote``. Will help you keep track 
 
 **README.md** will have links to all your notes on the Github repo.

TODOS:
- [ ] Sorting tags:
  - [ ] Sort the names by tag.
  - [ ] Sort the names by date.
  - [ ] sort the names by name (alphabetically)
- [ ] Delete ``*.md`` file ``*.cson`` has been deleted.
- [ ] Brings in oops.
- [ ] 😢😢😢 Anything other than ``INTERACTIVE`` is executed twice, dunno why pliz halp.
## Thanks to this repo:
- [pycson](https://github.com/avakar/pycson)
  - This helped in saving me alot of time.