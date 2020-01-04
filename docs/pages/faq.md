---
layout: page
title: Frequently Asked Questions
author: John Graybeal
permalink: faq
---

Here are our always-in-progress Frequently Asked Questions for CEDAR. Got a question? [Contact us](https://metadatacenter.org/contact "Contact us")!

**What is CEDAR good for?**

The CEDAR Workbench can be built into an existing metadata or data processing pipeline, help you submit metadata to an existing repository, or serve as a full-service metadata repository. It can be used to collect metadata following any specified template (form). It has also been useful for capturing metadata models or structures, with the added benefit of testing those models quickly using real data.

If you want to submit your metadata (even including data) to a particular domain repository, contact us about your interest; we are always evaluating which repositories to add next. See our Orientation for details.

**How do I get an account on CEDAR?**

Just go to the site (https://cedar.metadatacenter.org), where you will see a login screen. You can register using the Register link on that screen (just above the red Google icon), using your social media account or email address. That's it—you can start using CEDAR now!

I can't figure out what to do! How do I create a template or fill one out?
If you want to create a template that people can then use, go to your home directory (using the Home button at upper left). To create a new template (or anything else) move the mouse pointer to the red button in the lower right, wait for the options to pop up, and select what you want to create.

To fill out some metadata for a template, you'll need to find the template you're providing metadata for (hint: you can search for it), then control-click or right-click on the template and select "Populate" to generate a form to fill out. (If someone else has given you a link to fill out a CEDAR template, just go to that link in your browser. Once you're logged in you'll be in the Metadata Editor, ready to start filling out metadata.

For more startup information, go to our tools-training/training-cedar CEDAR training page, or to our CEDAR support page.

**What makes CEDAR forms so special? Google forms/SurveyMonkey surveys can do most of this.**

CEDAR is a little bit richer in some ways than Google forms or Survey Monkey surveys, and CEDAR adds two things in particular: real-time semantics, and metadata smarts.

With CEDAR semantics, you control exactly what terms can satisfy a query—and as soon as the source ontology changes, users see the updated list in the drop-down choices. By connecting your questions to other questions on the same subject, and connecting your answers to other answers that mean the same thing, these semantic relations can be exploited in the resulting metadata. As CEDAR collects more metadata for more standards and external systems, those connections will become more valuable as you ask about existing metadata (or build new CEDAR templates!).

And CEDAR knows a lot about entering metadata. Sure it can give a list of (semantically precise!) controlled terms to choose from, and auto-suggest completions for you. But it can also learn and share how the community filled out those forms, to help you check your own work. And using CEDAR, your lab manager can pre-configure a form for the team to use, hiding all the irrelevant fields and pre-setting defaults, to make your job faster.

Plus, over time CEDAR developers will be adding more time savers, like pulling in metadata from other sources, or validating your metadata against domain-specific rules. You'll get these features for free as soon as they are available.

**What format is the metadata saved in? How can I access it?**

We save the metadata as JSON-LD (in a Mongo database). We make it available (to those with access privileges) via the user interface, in both JSON-LD and the equivalent RDF Click on the format (at the bottom of the screen) to choose how you want to view it.

You can also access the metadata via the CEDAR API, in both of these formats, and in a "condensed JSON" format. That last format gets rid of lots of the link information (including much of the rich semantics).

**Is CEDAR open source, and if so, does it plan to continue to be open source?**

Yes, and yes. You can find CEDAR source code at https://github.com/metadatacenter, and technical documentation at https://metadatacenter.github.io.

**Can you make it easier to work with templates and elements, e.g., nesting a template within a template?**

Yes, but not yet. Right now, only an element or field can be included within a template. We have many feature ideas to make it easier to nest resources, including "live" resources.

**I have a system that already has a collection of metadata. Can I put that into CEDAR without retyping everything?**

Yes! The CEDAR APIs allow you to post your metadata content to CEDAR. You will need to define a template that will support your metadata content, and then format your metadata to match the corresponding CEDAR instance. One common way to do this is to create the template (the metadata form) the way you want it, then create an instance (one filled out metadata resource) using dummy data. You can inspect the format of the dummy instance (either downloading via API, or copying the text from the JSON-LD selector at the bottom of the instance form) in order to obtain the pattern that your instances will need to follow.

Our example repository on GitHub shows how to generate Java classes that produce CEDAR instances conforming to a particular template. You would need to write code to read the data from your XML archive and then use the API of the generated Java classes to copy values from your XML metadata into the Java object, which would then get serialized as JSON-LD.

**What is the 'link' fieldtype for?**

This is appropriate when you know the result has to be a URL, or some other type of IRI (the internationalized, generalized form of a URL). Unlike text fields, this field type validates the metadata entry to make sure it’s an IRI, and it produces appropriately typed RDF in the resulting metadata.

**What do you use for your identifiers?**

We mint UUID-based IRIs to identify all our artifacts (metadata templates, metadata instances, folders, and even users). You can see the identifier in the URL for the page you’re on. In a CEDAR page with a URL that looks like this:
```
https://cedar.metadatacenter.net/templates/edit/https://repo.metadatacenter.net/templates/226d6778-5978-4d55-a284-d8e7ec522ca5?folderId=https:%2F%2Frepo.metadatacenter.net%2Ffolders%2F4036e319-5bb7-493f-8fe5-31a004f65a94
```
you will see the first identifier string, like https://repo.metadatacenter.net/templates/226d6778-5978-4d55-a284-d8e7ec522ca5. This is the identifier for your artifact, in this case a template.

Note that the template identifier will not (yet) resolve in your browser if you do not prefix it with the appropriate CEDAR context, e.g., in this case `https://cedar.metadatacenter.net/templates/edit/`.

**How do I look up all instances of a template?**

Use the API search feature with the identifier of the template to find all the related instances. See the linked documentation for the details.

**How do I enter diacritics and other special characters?**

You should be able to enter them the same way you would in any other text entry in your computer—use the character chooser, or change your keyboard (both software tools are part of the computer operation system), or copy the special characters from another document and paste them into CEDAR. Please tell us if there is a CEDAR field that does not handle them correctly.

**Can I deploy CEDAR in my own computing environment?**

This is our intention, but CEDAR is not yet deployable in this way. We have Dockerized CEDAR so that we can deploy it internally, but can not release it for external use until we have addressed some engineering and policy issues. Contact us if you want more information about the release of a Dockerized version of CEDAR.