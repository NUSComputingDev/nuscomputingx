# NUSComputing.com Website
> the new, lightweight NUSComputing.com

## General Guide

### Requirements

* [hugo](http://gohugo.io)

### Running for the first time

Other than installing the requirements, there is nothing to do!

### Developing

In order to view your changes, you will need to build the source files and serve them (as viewing them using the `file` protocol might be quite wonky).

Don't fret, however! There is an easy way to do so, using Hugo's built-in server. This is the preferred method as it will automatically build and reload any changes you have made after spinning up the server.

You may want to run Hugo's server with the following flags, like so:

``` bash
$ hugo server -w -t hugo-agency-theme
```

### Testing

As Hugo is a static website generator, there are currently no automated test suites. Use your eyes to test.

### Production/Build

Once you are satisfied with the results, you can build the static website using the following command:

``` bash
$ hugo
```

The result will be placed in the `docs/` directory.

## Development/Website Guides

### Adding New Event to Event Page

1. Open terminal in root folder, create new event type markdown file by typing:
``` bash
$ hugo new event/<event name>.md
```
2. Open the Markdown file in your favourite editor.
Fill in the file with the event details as follows:
``` Markdown
+++
externalLink = <link to event page>
image = <filename of image (in ./static/img/event)>
modal = <modal ID>
title = <title>
+++

<description of event>
```
3. Commit, push and make a Pull Request to the repository.
