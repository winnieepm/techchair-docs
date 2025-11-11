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
 

# testing locally
Good coding practices recommend always testing your code offline before pushing new changes to GitHub to avoid uploading incorrect code or merging issues. 

ACH uses [11ty](https://www.11ty.dev/), a static site generator framework, to build its websites. You need to install **11ty** inside the website's folder to build your site and test it locally.

### for macs
1. Open the `Terminal` app and navigate to the location of the ACH conference website folder in your computer.

2. Once there, make sure you have the [Node Package Manager (NPM)](https://www.npmjs.com/) installed using the command `npm --version`. You can run and edit your **11ty** installation with this tool. Use Homebrew to install **NPM** if the previous command doesn't yield any results. 

3. Follow the step-by-step instructions on **11ty**'s **[Get Started](https://www.11ty.dev/docs/)** guide after **Step 2: Install Eleventy**.  

4. After installing **11ty**, test it on your computer to ensure everything works. In a command-line or **Terminal** window, go to your website's local folder and enter this command: `npx @11ty/eleventy --serve`. Once 11ty is done building the site, it will launch it on one of your computer servers and display an address similar to this: `http://localhost:8080/`. Open it on your browser to interact with your website. 

**Note: You may encounter a `Cannot GET` error. This means you have not set a language for the site. Simply add `/en` or `/es` at the end of the web address.** 


# content directory structure
The current setup for the ACH conference website is bilingual. Main content for the website is inside an English (`en/`) folder and translated in Spanish inside `es/`. If you can't update both, prioritize updating the markdown (`.md`) files inside `en/`.


