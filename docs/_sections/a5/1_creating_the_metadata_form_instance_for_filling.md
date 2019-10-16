---
layout: section
title: Starting the Metadata Form (Instance) for Filling
author: John Graybeal
status: In Progress
chapter: a5
chapter_url: /basic_topics/a5_filling_out_creating_metadata/
chapter_title: Filling Out Metadata

---
## **CEDAR's Metadata Instance**

In CEDAR, the forms to fill out with metadata are created as what we call metadata forms,
or to avoid confusion with templates, Metadata Instances or Instances.
The instances contain provided answers for each of the fields, 
and if the answers are unique identifiers for controlled terms,
the instances also contain the labels so that tools can display the values without performing a lookup.
When instances allow multiple entries for a field or element, 
entered values are stored in arrays. 
CEDAR stores all of this information in JSON-LD-formatted documents

CEDAR instances contain contextual metadata describing the instance, 
just as templates contain contextual metadata for template artifacts. 
One of those contextual fields specifies the CEDAR Metadata Template (and its version)
from which the instance was created. 

CEDAR instances do not contain detailed descriptions of the questions being asked,
nor details about the possible answers for those questions. 
Anyone who wants this information can use the identifier of the instance's source template
to get a copy of the instance and look up those values.  

## **Creating the Instance**

CEDAR offers several strategies for initiating a metadata form. 
These are described below according to the needs they satisfy, 
and ordered from simplest to most complex.  

### **Via a Web Link (An External IRI)**

In this scenario, the template creator has obtained a web link (an IRI) that, 
when entered into a browser or included clicked on as a link in a web page,
will create a metadata instance for that template. 
_TODO_: Reference or create the information on creating that link._
A logged-in user will proceed directly to the Metadata Editor with 
the newly created instance already opened.

If the user activating the link does not have a CEDAR account or is not logged in, CEDAR will redirect 
the person's browser to the CEDAR authentication page. 
At that point the user can log in or register for an account, and will be returned to
the Metadata Editor with the newly created instance already opened.

_TODO_: ![](https://github.com/metadatacenter/cedar-manual/raw/master/docs/assets/imgs/share-settings-find-your-group-20190909.png){:width="75%"}

### **Via a Web Link (An External IRI)**

In this scenario, the template creator has obtained a web link (an IRI) that, 
when entered into a browser or included clicked on as a link in a web page,
will create a metadata instance for that template. 
_TODO: Reference or create the information on creating that link. Include example_
A logged-in user will proceed directly to the Metadata Editor with 
the newly created instance already opened.

If the user activating the link does not have a CEDAR account or is not logged in, CEDAR will redirect 
the person's browser to the CEDAR authentication page. 
At that point the user can log in or register for an account, and will be returned to
the Metadata Editor with the newly created instance already opened.

### **From a Workspace view of the template**

This is the most common way to create an instance.
If the workspace doesn't have a view of the template, navigate in the workspace or
perform a search to bring the template into view in the List or Cards workspace view.

There are two variants to create a new metadata instance from the Workspace view: 
either click on the metadata tag to the right side of the template box, or 
click on the dropdown menu (the kebab, *:*) and select Populate Template.

_TODO_: highlighted graphic
![](https://github.com/metadatacenter/cedar-manual/raw/master/docs/assets/imgs/share-settings-find-your-group-20190909.png){:width="75%"}

### **From an existing instance made from that template**

This is the most common way to create an instance.
If the workspace doesn't have a view of the template, navigate in the workspace or
perform a search to bring the template into view in the List or Cards workspace view.

There are two variants to create a new metadata instance from the Workspace view: 
either click on the metadata tag to the right side of the template box, or 
click on the dropdown menu (the kebab, *:*) and select Populate Template.

_TODO_: highlighted graphic
![](https://github.com/metadatacenter/cedar-manual/raw/master/docs/assets/imgs/share-settings-find-your-group-20190909.png){:width="75%"}

### **From an API call to CEDAR**

This is the most common way to create an instance.
If the workspace doesn't have a view of the template, navigate in the workspace or
perform a search to bring the template into view in the List or Cards workspace view.

There are two variants to create a new metadata instance from the Workspace view: 
either click on the metadata tag to the right side of the template box, or 
click on the dropdown menu (the kebab, *:*) and select Populate Template.

_TODO_: highlighted graphic
![](https://github.com/metadatacenter/cedar-manual/raw/master/docs/assets/imgs/share-settings-find-your-group-20190909.png){:width="75%"}


