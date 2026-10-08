---
layout: post
title: The R Package: gh
subtitle: Excerpt from Soulshaping by Jeff Brown
cover-img: /assets/img/path.jpg
thumbnail-img: /assets/img/thumb.png
share-img: /assets/img/path.jpg
tags: [books, test]
date: 2026-10-08
---

**The R package gh provides an interface between R and the GitHub API, making it possible to send requests to GitHub directly from R.**

```
</>R
library(gh)
```


**The API returns information about the repository, including its name, description, number of stars, and number of forks. Because the response is returned as an R object, I can access individual pieces of information using $.**

# What type of data does it return?

The GitHub API uses **JSON(JavaScript Object Notation)** to send information. The gh package processes the API response and makes the information available as R objects, such as lists. This allows the data to be accesses and analyzed within R.

**GitHub -> GitHub API -> JSON -> gh package -> R**

One benefit of using an API is that you don't have to manually collect information from GitHub. I can use R to request the information I need and then use it for analysis. This could be usefl when working with multiple repositories or when trying to analyze activity across GitHub projects.


