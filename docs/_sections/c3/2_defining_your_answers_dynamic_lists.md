---
layout: section
title: Defining Your Answers - Dynamic Lists
author: John Graybeal
status: In Progress
chapter: c3
chapter_url: /cedar_templates/c3_more_fair_templates_using_semantics/
chapter_title: More FAIR Templates Using Semantics
---

Now we will show you exactly how to create questions 
that have very precise answers, using CEDAR's semantic tools.
You don't have to know semantics to use these tools—
we'll give you some tips (in [Choosing Controlled Terms](https://metadatacenter.github.io/cedar-manual/sections/c3/3_choosing_controlled_terms/) that help you find good answers for your questions,
and know they are good enough for your needs.

For you semantic experts, we provide advanced details elsewhere in this User Manual:
* [Tips for Template Creation: Term Discovery/Selection](https://metadatacenter.github.io/cedar-manual/sections/c5/term_discovery_selection/)
* [Advanced Template Topics:More Semantics](https://metadatacenter.github.io/cedar-manual/sections/c4/more_semantics/)

In this section we outline the mechanical steps to find, select, and even create terms. 
The next section will tell how to figure out which terms are good ones to use.

This section (except the Customization subsection at the end)
walks you through CEDAR interfaces that work hand-in-hand with the 
[BioPortal ontology repository](https://bioportal.bioontology.org). 
This repository contains over 800 public terminologies that offer precise semantic content
you can use for your metadata collection process. 
Even the addition of Values and Value Sets uses BioPortal to store those concepts.
But if BioPortal does not contain a terminology that you want to use, you can add it!
See the subsection called "Adding Content to BioPortal" in the [More Semantics](https://metadatacenter.github.io/cedar-manual/sections/c4/more_semantics/) section for more information on this process.

All the following sub-sections assume you have created a basic text field, 
clicked on the Values tab for your field,
and clicked on the Add button to bring up the term search dialog box, 
as described in [Adding Fields](https://metadatacenter.github.io/cedar-manual/sections/c2/2_adding_fields/).

## Basic Interactions

You may want to add individual terms or whole collections of them. 
First we will work at the level of individual terms, and 
progress to finding and adding collections of terms.


### Searching for Terms

![](https://github.com/metadatacenter/cedar-manual/raw/master/docs/assets/imgs/search-for-terms-list-results-20191229.png){:width="80%" class="centered"}
As soon as you hit the Add button in the Values tab of a CEDAR field,
CEDAR opens a new search window, pre-configured with the name in your field, 
and the search for terms begins immediately.
In this case, the name is "Study Type", and a set of results has been returned.
You can see each term in the scrollable list—the most likely terms are listed first.

You can change the search terms by typing in the search field. 
If you search doesn't begin immediately, click on the magnifying glass to start it.
The results list updates as more results are found,
and higher-value results may be inserted in front of results you are looking at.
Usually all the results are obtained quite quickly.
(A maximum of 500 results may be obtained.)

![](https://github.com/metadatacenter/cedar-manual/raw/master/docs/assets/imgs/search-for-term-advanced-options-20191229.png){:width="80%" class="centered"}
You may want to refine the search to meet particular needs.
By clicking on the settings gear at the right of the search field,
you will see a set of Advanced Search Options.
The first option, to search for a term anywhere in BioPortal, is pre-selected.
(We will discuss the other 'I want to…" options in later subsections.)

For now, we want to focus on the "Narrow your search to specific ontologies" field.
If you know the ontologies in BioPortal that you want to use for your terms,
you can enter them into this field. 
Start typing either the ontology acronym or its full name, 
and CEDAR will offer a list of the matching ontologies.
Click on the one that you want to include as a restriction,
and its acronym will appear in the field.

![](https://github.com/metadatacenter/cedar-manual/raw/master/docs/assets/imgs/search-for-term-restrict-ontologies-20191229.png){:width="80%" class="centered"}
You can begin typing again in the field, and select another ontology,
until you have found all the ontologies you want in your restriction list.
In this case, we have selected the ontologies with the acronyms CTO and NCIT.
This technique can be used to see more terms in the given ontologies,
or to exclude any other ontologies from being considered.

### Reviewing Found Terms

Now that you have some terms, you may want to take a closer look at the 
![](https://github.com/metadatacenter/cedar-manual/raw/master/docs/assets/imgs/search-for-terms-open-branch-20191229.png){:width="80%" class="centered"}

![](https://github.com/metadatacenter/cedar-manual/raw/master/docs/assets/imgs/search-for-terms-show-details-20191229.png){:width="80%" class="centered"}

### Selecting Terms, Branches, or Ontologies

![](https://github.com/metadatacenter/cedar-manual/raw/master/docs/assets/imgs/search-for-branch-20191229.png){:width="80%" class="centered"}

![](https://github.com/metadatacenter/cedar-manual/raw/master/docs/assets/imgs/select-branch-for-addition-20191229.png){:width="80%" class="centered"}

![](https://github.com/metadatacenter/cedar-manual/raw/master/docs/assets/imgs/search-for-ontology-20191229.png){:width="80%" class="centered"}

![](https://github.com/metadatacenter/cedar-manual/raw/master/docs/assets/imgs/search-for-value-set-20191229.png){:width="80%" class="centered"}

## *Adding Your Own Terms and Value Sets*

### About Provisional Terms

### Adding your Own Single Term(s)

![](https://github.com/metadatacenter/cedar-manual/raw/master/docs/assets/imgs/create-term-20191229.png){:width="60%" class="centered"}

![](https://github.com/metadatacenter/cedar-manual/raw/master/docs/assets/imgs/create-term-description-20191229.png){:width="60%" class="centered"}

![](https://github.com/metadatacenter/cedar-manual/raw/master/docs/assets/imgs/create-term-linked-to-existing-20191229.png){:width="60%" class="centered"}

### Composing a List of Terms

![](https://github.com/metadatacenter/cedar-manual/raw/master/docs/assets/imgs/create-value-set-definition-20191229.png){:width="60%" class="centered"}

## *Customizing What You Have*

### Rejecting Terms

### Putting Favorites First
