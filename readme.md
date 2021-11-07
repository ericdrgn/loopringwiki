# Adding Content

## Building Sidebars

To add a page to the wiki you will first need to modify the gridsome.config.js file. The created sidebars are API, FAQ, and Learn. To add to a side bar you will need to add a line to each section you are adding a page to. For example the below is the "Learn" sidebar structure in its entirety.

```
{
        name: 'learn',
        sections: [
          {
            title: 'v3.6',
            items: [
              '/learn/',
              '/learn/deploymentmainnet/',
            ]
          },
           {
            title: 'Walkthroughs',
            items: [
              '/learn/onboarding/',
              '/learn/liquidity/',
              '/learn/wallet/',
              '/learn/avoidfees/',
            ]
          },
          
```

As an example you if you wanted to add a page on "whatever" to the v3.6 section you would add the line '/learn/whatever/', to the structure as shown below.

```

{
            title: 'v3.6',
            items: [
              '/learn/',
              '/learn/deploymentmainnet/',
              '/learn/whatever/',
            ]
```

## Adding Pages

The sidebars are ogranized under /content/ and their respective names (/content/api/, /content/faq/, /content/learn/) and depending on which sidebar you are using you would add a markdown file to that specific directory. So using the example above we would go to /content/learn/ and create a file named "whatever.md" and then fill it with content.

### Additional Requirements for Pages

All pages must include something like the below format to be properly identified, added to the sidebar and correctly show previous and next pages. Make sure to use the appropriate paths and name of sidebar in this section.

```
---
description: ''
sidebar: 'learn'
prev: '/learn/'
next: '/learn/onboarding/'
---
```

In this example our "whatever.md" page comes after our "deploymentmainnet.md" page so we would have to change two things. First we would need to change the above for the "deploymentmainnet.md" page as "whatever.md" is now the next page.

```
---
description: ''
sidebar: 'learn'
prev: '/learn/'
next: '/learn/whatever/'
---
```

And since "whatever.md" is now the last page of that section it would look like the below.

```
---
description: ''
sidebar: 'learn'
prev: '/learn/deploymentmainnet'
next: '/learn/onboarding/'
---
```

### Page Structure

While the left hand sidebar needs to be manually created based on the steps provided the right hand sidebar is auto-generated based on the headers within the markdown file(s). The first header (#) becomes the title of the page and then every header after that (##, ###) continues to automatically build out the sidebar on the right hand side for each page.

# Credit

This was modified from the [Docc Template](https://github.com/mrcrmn/docc) for Gridsome. 
