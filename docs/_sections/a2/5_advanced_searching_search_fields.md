---
layout: section
title: Advanced Searching - Search Fields
author: John Graybeal
chapter: a2
---

This section contains some examples of the query syntax that can be used to find template instances by field name and/or value. 

Suppose the following template instance:

![](https://github.com/metadatacenter/cedar-manual/raw/master/docs/assets/imgs/field_search_example.png){:height="100%" width="100%"}

Examples of queries that will retrieve the instance above:

- Search by field name and value:

  `title:statistics`
  
  `publisher:"City of New York"`
  
- Search by field name (any value):

  `publisher:*`
  
- Search by field value (any name):

  `*:"New York"`
  
- Boolean queries (e.g. Title="Statistics" AND "New York"):

  `title:Statistics OR title:Math` *(the OR is optional)*
  
  `title:(Statistics OR Math)`
  
  `title:Math OR (title:Statistics AND publisher:"New York")`
  
  `Dataset OR disease:CRC`
  
- Wildcard queries: 

  - One or more characters: `title:stat*`
  
  - Single character: `title:stat?stics`
  
- URLs: 

   `url:https://catalog.data.gov/dataset/demographic-statistics-by-zip-code-acfc9`
   
- Ontology terms: 

    - Search by term label: `topic:statistics`
    
    - Search by term URI: `topic:http://edamontology.org/topic_2269`
