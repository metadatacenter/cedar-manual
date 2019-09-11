---
layout: section
title: Building Shareable Metadata Creation IRIs
author: John Graybeal
chapter: b1
status: Ready
---

Building on the other sections in this chapter, we briefly describe how to create an IRI 
that will launch a fresh appropriate metadata creation form for your template. 

Given a template IRI of the form https://repo.metadatacenter.org/templates/f7d62955-ed10-4912-b4db-1b366ad4ff00 (not a real template!),
preface it with the metadata creation IRI base https://cedar.metadatacenter.org/instances/create/.

This gives us a URL like 
`https://cedar.metadatacenter.org/instances/create/https://repo.metadatacenter.org/templates/f7d62955-ed10-4912-b4db-1b366ad4ff00`
which when clicked would launch CEDAR, login (or create account for) the user if necessary, 
and put the user into a new metadata creation form for that template. 

Because there is no 'return folder' specified in this URL, 
when the user saves the created metadata, it will be put into his or her home folder, and the user will be returned to that folder.
If the user will have write access to a particular folder where this metadata should go, appending the folderID 
(with `?folderID=`and the encoded ID of the target folder) will result in the saved metadata going into that folder, 
(though the user may not realize how that happened or how to return to it).
