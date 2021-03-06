---
title: How to add a wiki homepage, sidebar, and TOC in Google Code
date: "2009-07-01"
url: /blog/2009/07/01/how-to-add-a-wiki-homepage-sidebar-and-toc-in-google-code/
categories:
  - Open Source
  - Web
---
I just adore Google Code. But the default wiki view (a list of pages, sorted by last-modified) is lacking something. Fortunately, it's fixable. Here's the before:

![Default wiki list](/media/2009/07/Screenshot-Wiki-Pages-maatkit-Google-Code-Mozilla-Firefox.png)

And here's the after:

![Wiki with sidebar and default page](/media/2009/07/Screenshot-Wiki-Pages-maatkit-Google-Code-Mozilla-Firefox1.png)

Here's how:

1.  Create a wiki page called TableOfContents, or something like that. Using normal wiki syntax, enter links and text for your table of contents. The best way to do this is to use bulleted lists to organize and outline the pages. Keep in mind that we'll use this same text for the sidebar, so keep it brief.
2.  Go to Administer/Wiki and enter that wiki page's name in the "Wiki Sidebar" box. Save the changes.
3.  Go to Administer/Tabs and enter the same page in the Wiki box. Save the changes.

Now both the wiki "homepage" and the sidebar will contain the page you created. No more ugly list-of-pages. And as you navigate through the wiki pages, the sidebar automatically expands and closes the outline to show where you are.

If you want, you can use a different homepage and sidebar, but I've found that it works well for me to use the same page for both. It's a preference, that's all.

There's one more trick I'd like to share: you can add the text `<wiki:toc />` at the top of any page to create a small table of contents for that page. There are ways to customize it---check the documentation for more options.


