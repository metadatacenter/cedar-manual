---
layout: section
title: API: Accessing Metadata Instances
author: John Graybeal
status: Ready
chapter: b2
chapter_url: /advanced_topics/b2_cedars_api
chapter_title: CEDAR's API
---

There are several API methods that can find and return metadata instances. 
Note that in the API, metadata instances are called Template Instances
(template_instance in the method names). 
The API refers to an actual CEDAR template as a Template, 
though some might call it a 'template instance'. 
We apologize for this semantic hiccup.

We cover a few of the most useful API methods for finding and obtaining
CEDAR metadata instances in this page. 

<h1>Overview</h1>

CEDAR offers a number of search methods that can return metadata instances.
Most of these return, for each discovered metadata instance, 
the description of the instance (in other words, that instance's metadata).
To obtain the actual metadata (values) contained in one of those instances,
you need to make a request for the specific instance using its `instance identifier`.

<h2>Search Methods</h2>

When performing searches via the API, just like searches in the UI,
you will only find artifacts to which you (identified by your API key) have access.
You must ensure the metadata artifacts you want searchable are visible
to the people or groups you need to find and access them—
either by explicitly giving those people or groups access to the artifacts,
or by giving Everyone group access to the artifacts,
or by putting the artifacts into a folder visible to those people, groups, or 
the Everyone group.

CEDAR administrators can arrange for all the artifacts of a particular template
to be visible to a particular group, contact us at cedar-support@metadatacenter.org
to make that request.

<h3>Finding metadata instances in CEDAR</h3>

[To be augmented]

<h3>Finding instances of a particular parent template</h3>

To find the set of metadata instances that have 
a particular metadata template as their parent,
you will use the [Search GET method](https://resource.metadatacenter.org/api/#!/Template32Instances/get_search).
*NOTE*: The Swagger documentation does not execute this example successfully.

The Search method has many parameters, but the key parameter for this command
are is_based_on, which specifies the parent template's `template identifier`, 
and resource_types, which *must be left blank*. (It is required in every other search
request except this one.)

When put this command and your template identifier into a curl request 
that you can run from your Unix command line, 
and a pretty-printing command is added,
you obtain something like the following:
```
curl -X GET --header 'Accept: application/json' --header 'Authorization: apiKey YOUR_API_KEY' 'https://resource.metadatacenter.org/search?version=all&publication_status=all&is_based_on=https%3A%2F%2Frepo.metadatacenter.org%2Ftemplates%2F5bf8d2bf-2f1c-4d77-a399-a2222157d894&sort=name&limit=100' | /usr/local/prettyprint
```

<h2>Retrieval Methods</h2> 

To retrieve a metadata instance, you will use the [Template Instance GET method](https://resource.metadatacenter.org/api/#!/Template32Instances/get_template_instances_template_instance_id). 
This method has two parameters: the template_instance_id 
(the instance_identifier mentioned earlier), and 
the desired format.

The template_instance_id should look very similar to the following:
  `https://repo.metadatacenter.org/template-instance/8bc64ab5-df6b-48c8-8c61-6c016245918e`
The final 32 characters are the unique part of the string.

When this is put into a curl request that you can run from your Unix command line, 
and a pretty-printing command is added,
you obtain something like the following:
```
curl -X GET --header 'Accept: application/json' --header 'Authorization: apiKey YOUR_API_KEY' 'https://resource.metadatacenter.org/template-instances/https%3A%2F%2Frepo.metadatacenter.org%2Ftemplate-instances%2Ffb8f0a9c-8ded-4d31-9d92-fb780ff6b4df?format=jsonld' | /usr/local/prettyprint` 
```




