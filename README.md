# ST2-bigfix-syntax-definition

## Description

This is the YAML source for a user-defined syntax definition for the relevance language. Relevance is one of the proprietary languages used by IBM Endpoint Manager (IEM), formerly known as Bigfix.

## Why? Nobody uses this..

Well, I do in my job. Since there isn't a proper fixlet debugger in my development OS of choice (OS X), and I use ST2 a lot for development, I decided to hack this up. It's pretty much a work in progress.

## Installation

- In the menu, navigate to Preferences-Browse Packages. In OS X, the preferences menu is a sub-menu under "Sublime Text 2" menu.
- Copy over the file bigfix_relevance.tmLanguage to the User folder there.

  In OS X, the exact folder is /Users/<username>/Library/Application Support/Sublime Text 2/Packages/User. Not sure in other OSes.

  In Windows, the exact folder is C:\Users\<username>\AppData\Roaming\Sublime Text 2\Packages\User.

- Restart Sublime Text 2.
- Bigfix Relevance syntax should be available in the menu under View-Syntax. Opening *.qna files in Sublime Text 2 should automatically use that syntax as well.

## Building from source

The steps below attempt to complement the steps from [Sublime Text documentation](http://docs.sublimetext.info/en/latest/extensibility/syntaxdefs.html). For more information, please read the Sublime Text docs.

- Install the AAAPackageDev package in Sublime Text 2.
- In the menu, navigate to Tools-Packages-Package Development-New Syntax Definition. A new YAML template should be created in a new tab.
- Copy over everything in bigfix_relevance.YAML-tmLanguage EXCEPT THE UUID FIELD.
- To build, hit Cmd+B (not sure for the shortcut for other OSes). Or in the menu, navigate to Tools-Build.
- Restart Sublime Text 2 (though sometimes not necessary).

## Bugs / Known Issues

None at the moment.

The scope names might not make sense. One of the tips I got when googling about what scope names I can use is to model it after a language I often use. Since I like and use Ruby, I just tried to fit it to Ruby's scope names, just to get good colourization.
