# TrelloSync

A Google Sheets Add-on (Apps Script) for the bulk production of Trello cards.

It uses the [GAS Trello API wrapper library TrelloApp] (https://github.com/andrewroberts/GAS-TrelloApp).

## Getting Started

* Create a new Google Spreadsheet on your [Google Drive] (https://drive.google.com);
* in the spreadsheet create a sheet called TrelloSync and create one row for each card, with one column for each of the board name, list name, card name and card description;
* click the custom menu option "Add-ons>TrelloSync>Create cards" to create the cards.

## Authorisation

The first time you execute any of the menu options you'll need to go through the Trello authorisation flow:

* A dialog in the sheet will instruct you to look out for the first auth window, 

* a new window is automatically opened where you need to click on the link to open the Trello auth window: "Click to authorize Google Apps integration", if you are not logged into Trello you'll be asked to do so;

* in the Trello auth window - "Let TrelloApp use your account?" - click "Allow";

* You should now see "Google Apps integration authorized for user:" and your email address;

You can now close this window and re-attempt the menu action.

It is possible for the app's permission to be revoked from within Trello in which case whenever you try and create new cards TrelloSync will simply report "0 cards created". In this case use "TrelloSync>Reset" and then the next time you attempt to contact Trello you'll run through the auth flow again.

## Support 

Contact [andrew@roberts.net](mailto:andrew@roberts.net) or check out [the issues page] (https://github.com/andrewroberts/TrelloSync/issues).

You can [follow me on twitter] (https://www.twitter.com/andrewroberts6) or [on my blog] (http://www.andrewroberts.net/category/computing/) for the latest updates.

## Developers

The source code is open source and released under GPL v3.

[A copy of v0.1 of the Google Apps Script can be found here] (https://script.google.com/d/1wpId9rciaxL0R8e6Qc1NrAapWtzx-kIabUrEKHGXKuFOobYzZpNoNShf/edit?usp=sharing).
