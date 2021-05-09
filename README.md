# About
A template for creating foundry modules using typescript. Project files are setup to be hot reloaded.
Information on hot module replacement: https://webpack.js.org/concepts/hot-module-replacement/

# Setup:
- Run npm install
- Rename module.ts to your chosen module name.
- Rename the references to module.ts in webpack.config.js file. (Line 26)
- Fill in module.json with actual information.
- Create a symantic link between the dist/ folder to a module folder in FoundryUser/Data/modules/[MODULE_NAME]  
--	Instructions (for windows) 
--	Open a command prompt and navigate to FoundryUser/Data/modules   
--	Run: mklink /D MODULE_NAME [DEVELOPMENT_PATH]/dist  

A note on typescript, it is completely optional and if you do not wish to use then rename any .ts files and their references to .js.

# Usage:
Development: 
To run with hotswap enabled run the command: npm run start

Release:
To ready the project for release run the command: npm run build:production

CD/CI:
This template is setup with automatic github release, developed by League of Foundry Developers in
their FoundryVtt-Module-Template. https://github.com/League-of-Foundry-Developers/FoundryVTT-Module-Template 

# Credits:
Used webpack and setup files as reference: https://github.com/anvil-vtt/FateX 
Used github workflow and template reference: https://github.com/League-of-Foundry-Developers/FoundryVTT-Module-Template
