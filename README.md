# RSS Aggregator

This is a Java program that reads multiple RSS feeds and generates a nicely formatted HTML page of links for each feed, plus an HTML index page with links to the individual feed pages.

## Problem Statement

The task is to update the RSS Reader program so that it reads multiple RSS feeds and generates an HTML page of links for each feed, plus an HTML index page for the name of an XML file containing a list of URLs for RSS v2.0 feeds and for the name of an output file in which to generate an HTML page with links to the pages for the individual RSS feeds.

## Input XML Document Format

The input XML document has the following structure:

```xml
<feeds title="Title for index page">
  <feed url="the feed source URL" name="name of feed for index page"
    file="name of HTML file for feed" />
  <feed url="..." name="..." file="..." />
  ...
</feeds>
```

- The top-level tag, `<feeds>`, has a required attribute, `title`, whose value is the title to be used in the index page.
- Nested inside the top-level tag are 1 or more `<feed>` tags with the following required attributes:
  - `url`: the URL of the RSS feed
  - `name`: the name to use for the link to the feed in the index page
  - `file`: the name of the HTML file in which to generate the feed's table of links to news items

## How to Run

To run this program, you need to have Java installed on your system.

1. Compile the program using the command: `javac RSSAggregator.java`
2. Run the program using the command: `java RSSAggregator`

You will be asked to enter the name of an XML file containing a list of URLs for RSS v2.0 feeds and the name of an output file.

## Author

This program is written by Adewale Adenle.
