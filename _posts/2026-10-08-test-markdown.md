---
layout: post
title: Introduction
subtitle: What is the GitHub API?
gh-repo: daattali/beautiful-jekyll
gh-badge: [star, fork, follow]
# tags: [test]
comments: true
---

Throughout this course, we learned about working with data and using R to interact with different tools and APIs. Since we worked closely with GitHUb why not explore the GitHub API and learn how it can help us access and analyze data from repositories!


## So what is the GitHub API?


**The GitHub API allows users to access information from GitHub programmatically. Instead of manually visiting a GitHub repository and looking through its information, we can use R to request that information directly.**


![GitHub API](/beautiful-jekyll/assets/img/how-to-interact-github-api.png)

It can retrieve information such as:

-Repostory information
-Users
-Issues
-Pull Requests
-Commits
-Stars and forks
-Repository activity

Here's an example code:

~~~
</>R
library(gh)

repo_info <- gh("/repos/r-lib/gh")

repo_info$name
repo_info$description
repo_info$stargazers_count
repo_info$forks_count
~~~

And here is the same code with a GitHub repository:

~~~
</>R
repo_info <- gh("/repos/mgarc427/montyhall")

repo_info$name
repo_info$description
repo_info$stargazers_count
repo_info$forks_count
~~~

```javascript
var foo = function(x) {
  return(x + 5);
}
foo(3)
```


## Boxes
You can add notification, warning and error boxes like this:

### Notification

{: .box-note}
**Note:** This is a notification box.

### Warning

{: .box-warning}
**Warning:** This is a warning box.

### Error

{: .box-error}
**Error:** This is an error box.
