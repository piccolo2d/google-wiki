

For the impatient website editor: [Jumpstart](http://piccolo2d.googlecode.com/svn/site/README.txt)

# Introduction

The End-User website is available at http://piccolo2d.mro.name (current refuge after piccolo2d.org got lost. See issue#248 (on Google Code))

# Domain

Domain owner is https://code.google.com/u/102889966713065468455/

# Content

All pages are [xhtml strict](http://www.w3.org/TR/xhtml1/), layout and formatting is done exclusively via [CSS](http://www.w3.org/TR/CSS21/). All links within the website are relative, all downloads refer to the google code downloads section.

[Liquid layout](http://www.useit.com/alertbox/screen_resolution.html) ensures excellent readability with a very wide range of monitor resolutions and browser window dimensions.

Javascript is used only where it brings significant benefit, namely to switch the code samples for Java and .Net.

Every page has a feedback link to ease error reporting.

## Template
The content was adapted from http://www.cs.umd.edu/hcil/jazz/ with friendly permission during issue 42 (on Google Code).

## Version Management

The **complete** website content is versioned in the project's svn repository: http://piccolo2d.googlecode.com/svn/site

**Caution**: The site contains a huge number of documentation html pages (>7000 files for .Net and Javadoc, maven reports, etc.).

Publishing a (unchanged but newly generated) set of maven reports consumes **10 MB** of svn repository space and the commit takes **over 1 hour**.

Maybe we pick a git hosting solution for versioning the website content in the future. I cloned the site repo to a public git repo at http://github.com/mro/piccolo2d.site. Feel free to have a look, but expect a 35MB download.

## Staging area

The [svn repository](http://piccolo2d.googlecode.com/svn/site) also serves as a staging area. Therefore the svn:mime-type of all files must be set correctly. The script http://piccolo2d.googlecode.com/svn/site/tools/svn-mime-types.sh helps to do that.

## Deployment

The content at piccolo2d.mro.name is served from a checked out working copy backed with http://piccolo2d.googlecode.com/svn/site

A [cron job](http://en.wikipedia.org/wiki/Cron) (at piccolo2d.mro.name) keeps the site up-to-date by running a mere "svn update" every 4 hours, namely a [crontab](http://en.wikibooks.org/wiki/Guide_to_UNIX/Explanations/Scheduling_Jobs#Crontab_format) pattern of
```
0 3,7,11,15,19,23 * * *
```
(CE(S)T Time)

# Tools

Alongside the website come some [tools](http://piccolo2d.googlecode.com/svn/site/tools/README.txt) to inject navigation into the static html pages and ensure consistently indented xhtml strict.

The navigation injection into a single html page is done [by a ruby script](http://piccolo2d.googlecode.com/svn/site/tools/inject_navigation.rb) that uses this [navigation data](http://piccolo2d.googlecode.com/svn/site/tools/navigation.txt).

Other tools set the [svn:mime-type property](http://piccolo2d.googlecode.com/svn/site/tools/svn-mime-types.sh) or [convert images from gif to png](http://piccolo2d.googlecode.com/svn/site/tools/giftopng.sh).