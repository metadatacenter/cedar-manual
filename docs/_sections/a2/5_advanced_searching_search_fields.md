---
layout: section
title: Advanced Searching - Search Fields
author: John Graybeal
chapter: a2
---
# Examples:

- Search by field name and value
  `title:statistics`, `publisher:"City of New York"`
- Search by field name (any value)
  `publisher:*`
- Search by field value (any name)
  `*:"New York"`
- Boolean queries (e.g. Title="Statistics" AND "New York")
  `title:Statistics OR title:Math (the OR is optional)`
  `title:(Statistics OR Math)`
  `title:Math OR (title:Statistics AND publisher:"City of New York")`
  `Dataset OR disease:CRC`
- Wildcard queries: 
  `title:stat*`
  `title:stat?stics`
- URLs: 
   `url:https://catalog.data.gov/dataset/demographic-statistics-by-zip-code-acfc9`
- Ontology terms: 
    `topic:statistics`
    `topic:http://edamontology.org/topic_2269`
