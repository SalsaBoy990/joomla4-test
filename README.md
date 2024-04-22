# Joomla 4 Starter project

TODO: Dockerize the project with these specs:
- PHP 8.2
- MySQL 8.0 +
- Apache 2.4 + / nginx 1.18 +


## Modifications

The `package.json` file and the `build` folder was imported from [the official Joomla repository](https://github.com/joomla/joomla-cms).
These are needed for compiling SCSS to CSS. Run this command to build css:

```shell
npm run build:css
```

Watch for changes:

```shell
npm run watch
```

In order to the compilation not to fail, in the file `your-path-to-the-project/build/build-modules-js/compilecss.es6.js`
comment line 43 out:

```php
/*`${RootPath}/installation/template`,*/
```

After installation, the installation is going to be removed, so the build script won't find the folder, and will throw an error.

A `.gitignore` file is added that is going to ignore most of the default Joomla files. As a result, this repository will


======

Joomla! CMS™

1- Overview
	* This is a Joomla! 4.x installation/upgrade package.
	* Joomla! Official site: https://www.joomla.org
	* Joomla! 4.4 version history - https://docs.joomla.org/Special:MyLanguage/Joomla_4.4_version_history
	* Detailed changes in the Changelog: https://github.com/joomla/joomla-cms/commits/4.4-dev

2- What is Joomla?
	* Joomla! is a Content Management System (CMS) which enables you to build websites and powerful online applications.
	* It's a free and Open Source software, distributed under the GNU General Public License version 2 or later.
	* This is a simple and powerful web server application and it requires a server with PHP and either MySQL, PostgreSQL or SQL Server to run.
	You can find full technical requirements here: https://downloads.joomla.org/technical-requirements.

3- Is Joomla! for you?
	* Joomla! is the right solution for most content web projects: https://docs.joomla.org/Special:MyLanguage/Portal:Learn_More
	* See Joomla's core features - https://www.joomla.org/core-features.html
	* Try out our free hosting service: https://launch.joomla.org

4- How to find a Joomla! translation?
	* Repository of accredited language packs: https://downloads.joomla.org/language-packs
	* You can also add languages directly to your website via your Joomla! administration panel: https://docs.joomla.org/Special:MyLanguage/J4.x:Setup_a_Multilingual_Site/Installing_New_Language
	* Learn how to setup a Multilingual Joomla! Site: https://docs.joomla.org/Special:MyLanguage/J4.x:Setup_a_Multilingual_Site

5- Learn Joomla!
	* Read Getting Started with Joomla to find out the basics: https://docs.joomla.org/Special:MyLanguage/J4.x:Getting_Started_with_Joomla!
	* Before installing, read the beginners guide: https://docs.joomla.org/Special:MyLanguage/Portal:Beginners

6- What are the benefits of Joomla?
	* The functionality of a Joomla! website can be extended by installing extensions that you can create (or download) to suit your needs.
	* There are many ready-made extensions that you can download and install.
	* Check out the Joomla! Extensions Directory (JED): https://extensions.joomla.org

7- Is it easy to change the layout display?
	* The layout is controlled by templates that you can edit.
	* There are a lot of ready-made professional templates that you can download.
	* Check out the template management information: https://docs.joomla.org/Special:MyLanguage/Portal:Template_Management

8- Ready to install Joomla?
	* Check the minimum requirements here: https://downloads.joomla.org/technical-requirements
	* How do you install Joomla - https://docs.joomla.org/Special:MyLanguage/J4.x:Installing_Joomla
	* You could start your Joomla! experience building your site on a local test server.
	When ready it can be moved to an online hosting account of your choice.
	See the tutorial: https://docs.joomla.org/Special:MyLanguage/Installing_Joomla_locally

9- Updates are free!
	* Always use the latest version: https://downloads.joomla.org/latest

10- Where can you get support and help?
	* The Joomla! Documentation: https://docs.joomla.org/Special:MyLanguage/Main_Page
	* FAQ Frequently Asked Questions: https://docs.joomla.org/Special:MyLanguage/Category:FAQ
	* Find the information you need: https://docs.joomla.org/Special:MyLanguage/Start_here
	* Find help and other users: https://www.joomla.org/about-joomla/create-and-share.html
	* Post questions at our forums: https://forum.joomla.org
	* Joomla! Resources Directory (JRD): https://community.joomla.org/service-providers-directory/

11- Do you already have a Joomla! site that's not built with Joomla! 4.x ?
	* What's new in Joomla! 4.x: https://www.joomla.org/4
	* What are the main differences between 3.x and 4.x? https://docs.joomla.org/Special:MyLanguage/What_are_the_major_differences_between_Joomla!_3.x_and_4.x
	* How to migrate from 3.x to 4.x? Tutorial: https://docs.joomla.org/Special:MyLanguage/Joomla_3.x_to_4.x_Step_by_Step_Migration
	* How to migrate from 2.5.x to 3.x? Tutorial: https://docs.joomla.org/Special:MyLanguage/Joomla_2.5_to_3.x_Step_by_Step_Migration
	* How to migrate from 1.5.x to 3.x? Tutorial: https://docs.joomla.org/Special:MyLanguage/Joomla_1.5_to_3.x_Step_by_Step_Migration

12- Do you want to improve Joomla?
	* Where to request a feature? https://issues.joomla.org
	* How do you report a bug? https://docs.joomla.org/Special:MyLanguage/Filing_bugs_and_issues
	* Get Involved: Joomla! is a community developed software. Join the community at https://volunteers.joomla.org
	* Documentation for Developers: https://docs.joomla.org/Special:MyLanguage/Portal:Developers
	* Documentation for Web designers: https://docs.joomla.org/Special:MyLanguage/Web_designers

Copyright:
	* (C) 2005 Open Source Matters, Inc. <https://www.joomla.org>
	* Distributed under the GNU General Public License version 2 or later
	* See License details at https://docs.joomla.org/Special:MyLanguage/Joomla_Licenses