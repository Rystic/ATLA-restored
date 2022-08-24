# Info

## Special Comments

Commit #599 introduced a new system of assignment marking (todos in the code), question marking, and a tagging system.

During the development of a mod, you don't always have time to do what you want to do right here and now.
That's why sometimes we need special comments.

## For VSCode Users

If you are developing with VSCode, then you should install an extension called [Better Comments](https://marketplace.visualstudio.com/items?itemName=aaron-bond.better-comments)
This extension Improves your code commenting by annotating some special words or marks with colors.

## List of special comments:

### General:

* <span style="color:#FF8C00"># todo:</span><span style="color:white">\<text\></span>- what must be done someday
* <span style="color:#3498DB"># ?question:</span><span style="color:white">\<text\></span> - some question to discuss with the team
* <span style="color:#98C379"># *note:</span><span style="color:white">\<text\></span> or <span style="color:#98C379"># *info:</span><span style="color:white">\<text\></span> - some useful or additional information about how to implement something mentioned in the <span style="color:#FF8C00">todo:</span>
* <span style="color:#FF2D00"># ! <span style="color:white">\<text\></span></span> - Important notes on working with an entity

### Tags:

This is done to find events with problems or dependencies more quickly.
Some blocks of code have special ***tags***, beginning with an exclamation point without spaces in words.

* <span style="color:#FF2D00"># !nevercalled</span> - events that declared, but never called somewhere else
* <span style="color:#FF2D00"># !nopicture</span> - events, or other entities without a picture
* <span style="color:#FF2D00"># !depends: <span style="color:#FF8C00">
\<list of events, decisions, etc\></span></span> - some commented events or other entities, like artifacts, were used <span style="color:#FF8C00">somewhere else</span>, but their usage was also commented, so if you uncomment these entitites, don't forget also to uncomment their usage in the code 
* <span style="color:#FF2D00"># !alternate</span> - Mention of an alternate start commands, or properties.

