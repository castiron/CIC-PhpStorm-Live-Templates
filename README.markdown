# TYPO3 Flavored Live Templates for PHP Storm

## Getting started

This repository is a little funky since PHP Storm's file structure for Live Templates isn't the easiest thing to integrate with a VCS. Nonetheless, the process for getting set-up isn't too bad. 

Here's what you're going to want to do:

* `cd ~/Library/Preferences/WebIDE10/templates`
* Now you need to exclude any existing Live Templates from being included in your repository. In my templates directory there was a file for 'Zen HTML.' That template isn't maintained in this repository so I exclude it, by adding the file path to a .gitignore, like this:
`echo "Zen HTML.xml" > .gitignore`
* Now initialize the a repo: `git init`
* Add the remote repo: `git remote add origin git@github.com:castiron/CIC-PhpStorm-Live-Templates.git`
* Pull everything down: `git pull origin master`

## What's Included

Currently there are three Live Templates in this bundle:

- Flexform
- Fluid
- TYPO3

Here's what's currently included in each template. 

### Flexform

* `flexCheck` Generates a flexform checkbox field.
* `flexDam` Generates a group field for selecting DAM records.
* `flexForeign` Generate a select field with options form a foreign table that you specify.
* `flexImage` Generate image upload field (not DAM aware).
* `flexInput` Basic text input
* `flexLink` Generates a text input field with link wizard.
* `flexOption` Generates a select option.
* `flexRepeat` Generates a repeating element container.
* `flexRoot` Generates a basic flexform structure.
* `flexRte` Generates an RTE enabled text field.
* `flexSelect` Generates a basic select field.
* `flexSheet` Generates a flexform sheet.
* `flexText` Generates an input field.

### Fluid

* `f:for`
* `f:formatHtml`
* `f:formatNl2br`
* `f:if`
* `f:image`
* `f:linkPage`
* `f:translate`

### TYPO3

* `t3debug` Prints a TYPO3 debug statement, although, you really should be using xdebug if at all possible!
* `tcaDamMM` Creates a TCA column configured for the DAM.
* `tcaDate` Creates a TCA date column.
* `tcaLink` Creates a TCA input field, with link wizard.
* `tcaText` Generates a TCA text field.

## Contributing

Add snippets to this! Make existing snippets better!