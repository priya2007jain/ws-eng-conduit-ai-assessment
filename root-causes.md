# Root Causes

Please copy-paste the final answer that you obtained from the AI for each question. The chat interface has a copy button that you can use to copy each message in Markdown format. Please do NOT include images or screenshots.

## Problem 1

**Problem**: The tags are broken up into individual characters on the post view page.

**Question**: What is the underlying issue that causes this problem to occur and from which component (file) of this project does this issue originate?

**Answer**: The issue is while saving the article its API response was considering each character instead of a comma separated string. 
File : apps/backend/src/article/article.service.ts
API : https://ubiquitous-garbanzo-69w6wjq9jr54f4pjg-4200.app.github.dev/api/articles/


## Problem 2

**Problem**: New tags  are not shown on the home page under "Popular Tags", even after a page refresh.

**Question**: What is the underlying issue that causes this problem to occur and from which component (file) of this project does this issue originate?

**Answer**: Tags which were mentioned in the new articles were not getting added to database in Tags table and hence not rendering in UI under "Popular Tags"
File : apps/backend/src/article/article.service.ts
API : https://ubiquitous-garbanzo-69w6wjq9jr54f4pjg-4200.app.github.dev/api/tags
