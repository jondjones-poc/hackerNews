# Introduction

In this task, you will implement a news reader. Your application will make it easy to browse
a list of articles featured on Hacker News. You will be expected to use React but beyond
this, you are free to make whatever technology choices you think best.
Your application should make use of the Hacker News API to provide a list of the most
recent stories. The documentation for this API is available at:

[https://github.com/HackerNews/API](https://github.com/HackerNews/API)

Quoting the README, "it's not the ideal public API". You are expected to account for these
limitations in your application, providing a beautiful user experience despite the limitations.
Equal focus will be given to the user experience and the quality of the code. Ultimately, we
care about building beautiful products for our users and so the experience you provide is
paramount.

**Live Site**: [https://hackernewsapi-poc.netlify.app/](https://hackernewsapi-poc.netlify.app/)

[![Netlify Status](https://api.netlify.com/api/v1/badges/69ad8625-6ed9-4765-a80a-efd14b3c1d89/deploy-status)](https://app.netlify.com/sites/hackernewsapi-poc/deploys)

## Requirements

Your solution should contain your source code and a README containing build and
deployment instructions. You may assume the engineer assessing your solution has
working Node.js and yarn installations.

## Packages

- React-content-loader
- Redux
- Thunk
- Styled-components

## Patterns

- Skeleton added on load to make it nicer when page loads
- Functional components
- Hooks
- Redux state management

## Approach 

To make a better experience for the user I used one of the hacker new aggregates.  This cut out me having to do unneeded queries back to the API, improving page load time.

To make the page more interesting I've added a sticky banner, there is also a skeleton when the data loads too slowly..  I also added in infinity scrolling with a spinner to save performance to. 

The site uses redux o manage the news state,  The idea was to add a filter reducer, to only return 5 result at the same time.

