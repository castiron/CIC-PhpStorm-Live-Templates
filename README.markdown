# TYPO3 Flavored Live Templates for PHPStorm IDE

## Getting started

This repository is a little funky since PHPStorm's file structure for Live Templates isn't the easiest thing to integrate with a VCS. Nonetheless, the process for getting set-up isn't too bad. 

Here's what you're going to want to do:

* `cd ~/Library/Preferences/WebIDE10/templates`
* Now you need to exclude any existing Live Templates from being included in your repository. In my templates directory there was a file for 'Zen HTML.' That template isn't maintained in this repository so I exclude it, by adding the file path to a .gitignore, like this:
`echo "Zen HTML.xml" > .gitignore`
* Now initialize the a repo: `git init`
* Add the remote repo: `git remote add origin git@github.com:castiron/CIC-PhpStorm-Live-Templates.git`
* Pull everything down: `git pull origin master`

## What's Included

Currently there are three Live Templates in this bundle:

* `Flexform`
* `Fluid`
* `FluidInline`
* `TYPO3`

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

* `f:alias` Generates an alias viewhelper tag 
* `f:checkbox` Generates a form checkbox  
* `f:cObj` Generates a cObject viewhelper tag 
* `f:crop` Generates a crop format viewhelper tag 
* `f:currency` Generates a currency format viewhelper tag 
* `f:date` Generates a date format viewhelper tag 
* `f:debug` Generates a debug viewhelper tag 
* `f:errors` Generates a for viewhelper iterating through form errors for a given property 
* `f:flash` Generates a flash  viewhelper tag
* `f:for` Generates fluid for each snippet 
* `f:form` Generates a form viewhelper tag 
* `f:gfor` Generates a grouped for snippet 
* `f:hidden` Generates a hidden field viewhelper tag 
* `f:html` Generates a HTML format viewhelper tag 
* `f:if` Generates an if snippet 
* `f:ifelse` Generates an if snippet around then and else viewhelper tags 
* `f:image` Generates an image viewhelper tag 
* `f:linkEmail` Generates an email link viewhelper tag 
* `f:linkExteranl` Generates an external link viewhelper tag 
* `f:linkPage` Generates a page link viewhelper tag 
* `f:nl2br` Generates a nl2br viewhelper tag 
* `f:ns` Generates a Fluid namespace declaration 
* `f:number` Generates a number format viewhelper tag 
* `f:password` Generates a password form field viewhelper tag 
* `f:radio` Generates a radio button form field viewhelper tag 
* `f:select` Generates a select form field viewhelper tag 
* `f:submit` Generates a submit form field viewhelper tag 
* `f:textarea` Generates a textarea form field viewhelper tag 
* `f:textfield` Generates a text form field viewhelper tag 
* `f:translate` Generates a translate viewhelper tag 
* `f:upload` Generates an upload form field viewhelper tag 

### FluidInline

* `if:if` Generates an inline fluid if snippet
* `if:translate` Generates an inline translate viewhelper tag

### TYPO3

* `inject` Generates an injectable extBase property and a corresponding inject method
* `t3debug` Prints a TYPO3 debug statement, although, you really should be using xdebug if at all possible!
* `ebdb` Prints an ExtBase var dump message, which is useful for debugging recursive, heavily nested  objects
* `tcaDamMM` Creates a TCA column configured for the DAM.
* `tcaDate` Creates a TCA date column.
* `tcaLink` Creates a TCA input field, with link wizard.
* `tcaText` Generates a TCA text field.
* `sqlSelect` Generates code needed for a direct SQL select query.
* `sqlInsert` Generates code needed for a direct SQL insert query.
* `sqlUpdate` Generates code needed for a direct SQL update query.
* `ipmatch` Checks if REMOTE_ADDR == the IP from specialbody.com.

## Contributing

Add snippets to this! Make existing snippets better!
