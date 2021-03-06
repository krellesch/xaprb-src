---
title: Stored procedure debugging in MySQL
date: "2012-11-01"
url: /blog/2012/11/01/stored-procedure-debugging-in-mysql/
categories:
  - Databases
---
I was just skimming through the latest "Meet the Experts" podcast from Oracle, whose topic is [debugging stored routines in MySQL](http://sqlhjalp.blogspot.com/2012/11/debugging-stored-routines-in-mysql.html). The tl;dr (tl;dl?) version is if you're working with Windows and .NET, you can install a Visual Studio plugin that lets you debug stored routines in the server via the .NET connection libraries. That's pretty nice, for those who are using that platform. The podcast is only a few minutes, so if you're interested, by all means listen to it, or take a look at the [documentation](http://dev.mysql.com/doc/refman/5.5/en/connector-net-visual-studio-debugger.html).

The ideal way to debug stored routines would be an API in the server, but that doesn't exist. Nevertheless, I remembered having seen some sort-of implementations of debugging at times in the past. My memory was that they used some workarounds to inject debugging code into the routines, using some things like special tables to communicate the values of variables and so on. I searched my quick-snippets file and did a brief web search, and turned up a lot more options than I remembered! In addition to the feature explained in the Oracle podcast, these products also offer stored procedure debugging of one type or another:

*   [Hopper](http://www.upscene.com/products.hopper.index.php) ([beta demo](http://www.upscene.com/products/hopper/demos/hopper_mysql_beta1.htm))
*   [The Illatis Stepin](http://marketplace.eclipse.org/content/illatis-stepin-debugger-mysql-procedures) plugin for Eclipse
*   [MyDebugger](http://mydebugger.com/)
*   [Devart dbForge](http://www.devart.com/dbforge/mysql/studio/demostutorials/debugging.html#debugging)
*   And, if you want to do it yourself, here's a pretty thorough walk-through from [BlueGecko](http://www.bluegecko.net/mysql/debugging-stored-procedures/)

I haven't used any of the above, and I'm not endorsing them, but I thought it might be helpful to have a list in one place. Did I miss any? 


