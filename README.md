# Node.js Template

A template repository for a [Node.js](https://nodejs.org/) project.
This includes scripts to get a development system setup on Windows, Linux or hopefully MacOS, although I don't own a Mac so I cannot be sure.

The version of Node.js can be specified in [.nvmrc](.nvmrc) but be aware that due to restrictions with [nvm-windows](https://github.com/coreybutler/nvm-windows) this needs to be the full version number e.g. 14.5.0 or v12.8.2.

## Scripts To Rule Them All

The following scripts will help you maintain your local development system.
There are bash scripts for Linux based systems, including MacOS or even Windows Subsystem for Linux.
Alternatively if running from PowerShell the ps1 versions will automatically be run instead.

### [script/setup](script/setup) ([script/setup.ps1](script/setup.ps1))

Used to set up a project in an initial state.
This is typically run after an initial clone, or, to reset the project back to its initial state.

### [script/update](script/update) ([script/update.ps1](script/update.ps1))

Used to update the project after a fresh pull.
This should include any database migrations or any other things required to get the state of the app into shape for the current version that is checked out.
