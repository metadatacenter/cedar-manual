---
layout: chapter
title:  CEDAR's API
author: John Graybeal
chapter: b2
status: In Progress
---

This chapter presents CEDAR's API, or Application Programming Interface. 
It covers the CEDAR API documentation, different ways to access the API,  
and detailed methods to access CEDAR information using the API, 
including retrieving metadata and submitting new metadata.

<h1>Introduction to the CEDAR API</h1>

CEDAR is written in a way that all of its services are accessible via a RESTful API.
A focused subset of those services are "open services",
intended for any CEDAR user to use as they wish.
In our CEDAR guide we will describe the use of these open services.

To use the CEDAR API you will need an API key, 
as well as the software tooling required to make queries directly to the API.
This tooling can be a simple operating system command like 'curl', 
the API Swagger documentation's built-in testing commands, 
an API accession tool, or a complete software application. 
Most of our documentation uses examples with curl to demonstrate API access.

You will need an API key to access the API.
You can find your key by creating your CEDAR account and logging in,
then navigating to your profile page.
Your API key, and basic information about using it, should be visible on this page.

In this manual we use the expression `YOUR_API_KEY` to stand in for 
the UUID string of characters that is your API key. 
Whenever you see YOUR_API_KEY in a command, 
replace that text with your API key before trying to use the command.


