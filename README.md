# sfdc_styling_gapafoundation
CSS styling to be uploaded into Salesforce for Volunteers4Salesforce. The limitation is that the html page is already stylized, so all styling must be done inside the CSS sheet.

![Demo image of the page](https://github.com/calvinshin/sfdc_styling_gapafoundation/blob/master/images/Current.png)

## Overview
Salesforce Volunteers For Salesforce (V4S) provides iframes that an organization can embed into other pages. The limitation is that all modifications on these iframes is generally done through the CSS file.

![Raw image stripped of all CSS](https://github.com/calvinshin/sfdc_styling_gapafoundation/blob/master/images/Raw.png)
Above is an image of the HTML page stripped of all CSS styling. While the html has some elements with classes, other elements do not. This requires child combinators in order to properly style the page.

## CSS Examples

### Child combinators
A combination of child combinators allow for modifying the table elements and then negating the modifications for other tables.
.cssInputFieldsColumn > div

### Content injection
By using ::before and the CSS style content, we are able to inject headers to divs.
