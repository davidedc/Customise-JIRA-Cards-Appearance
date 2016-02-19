## Summary
You can quickly customise JIRA cards appearance, based on almost any field of issues.

## More info
There is a supported way to inject javascript in each and every JIRA page served to users. This can be used to inject scripts to give a custom visualisation of your choice to any field visible in your cards (JIRA lets you choose three fields of your issues to be shown in the card). You can for example represent progress via a progress bar (instead of via numbers), or highlight specific situations via dedicated icons.

The solution consists in pasting javascript code in the JIRA "Announcement banner" configuration. This can be done by any administrator via the web UI.

The javascript code will check to actually render the visualisations only in a board (or many) of your choice.

This solution might or might not be the "best" long-term way to overlay visualisations of interest, but it's surely a quick way to prototype interesting visualisations.

##Example

The script in the .txt file of this project adds a "zombie" icon to issues that haven't changed state for more than a 100 days. This is far more effective than the default "dots" representation. The change is only done for a specified board.

You can see the result in the screenshot attached - see the zombie icons inside the red circles.

![adding zombie icon to stale issues](https://raw.githubusercontent.com/davidedc/Customise-JIRA-Cards-Appearance/master/readme-images/addIconsToCards.png)
