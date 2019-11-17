---
layout: section
title: Saving and Validating
author: John Graybeal
status: In Progress
chapter: a5
chapter_url: /basic_topics/a5_filling_out_creating_metadata/
chapter_title: Filling Out Metadata

---
_TODO_: reorganize if needed

## **Saving**

To save the instance, click on the Save button at the bottom right of the instance.

![](https://github.com/metadatacenter/cedar-manual/raw/master/docs/assets/imgs/share-settings-find-your-group-20190909.png){:width="75%" class="centered"}

While an instance is being edited in the Metadata Editor, it can be saved at any time.
If you have made changes and try to leave the instance without saving it, 
CEDAR will issue a warning. If you click Continue, any changes you made will be lost. 
Choosing Go Back will return you to the instance, where you can save it.

Since it is possible to close the browser window without getting the warning,
so we recommend saving your work frequently. 
Because there is no undo, should you need to recover a previous version of the document,
you will need to contact CEDAR staff to restore it.

_TODO_: verify this

At the top right of the instance, there are 3 icons that indicate the instance status.
The left-most icon (the circle) is filled when the instance is saved, 
but is hollow when there are unsaved changes.

## **Validation**

Whenever CEDAR saves an instance with entered content, it attempts to validate the instance
follows the JSON Schema specified by the template. 
On a successful verification, CEDAR issues a green "Instance saved successfully" notification.
If the verification fails due required fields being missing, 
CEDAR issues a report listing the missing fields.
If the verification fails due to a more fundamental error,
CEDAR issues a red "Instance not saved" message, 
along with basic error messages. 