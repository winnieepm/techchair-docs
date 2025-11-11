---
title:  Conference Website
description: Every conference has its own dedicated public website for accessibility, and a member-only instance of ConfTool to manage submissions, registration, and participant communications.
layout: libdoc_page.liquid
permalink: /content/conference-site/index.html
eleventyNavigation:
    key: Conference Website
---
This page only refers to the setup for the public website, and does not cover the ConfTool configuration. To setup the latter, check the [ConfTool]("#") section in this guide to learn more.

**Requirements: [11ty](https://www.11ty.dev/), [GitHub](https://github.com/), [Netlify](https://www.netlify.com/), [VS Code](https://code.visualstudio.com/) (or another code editor)**


# initial setup
1. Become a member of the ACH's organization GitHub account: [`achorg`](https://github.com/achorg) (if you haven't). Request an invitation from an admin or member of the organization account. They can add new authorized users by sending an invitation to other Github user's account handle or ID.

2. Fork the repository from the most recent conference and rename the new repo's name to `"achYYYY-website"` where `"YYYY"` is substituted by the upcoming conference year. Previous public websites from past conferences are stored in the ACH's organizational GitHub. 

3. Clone the new website repo to your computer so you can work on it locally. You can either use the `Git` command-line tool or use the [GitHub Desktop GUI](https://desktop.github.com/download/). 

4. Deploy the new website on Netlify. Log into the ACH's Netlify account using the credentials below, create a new, site and connect it to the Github repository. Netlify will automatically detect the `netlify.toml` file inside the GitHub repository to build and publish your website.
    ``` 
        username:  
        password: 

5. Copy the live link address for the website and add it to the `About` section of its GitHub repository.
