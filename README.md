# nuscomputingx
![nuscomputingx](https://img.shields.io/badge/nuscomputing-x-blue.svg)

## Development Guide

### Requirements

* [hugo](http://gohugo.io)

### Contributing

We follow the [Github Flow](https://guides.github.com/introduction/flow/).

### Developing

In order to view your changes, you will need to build the source files and serve them.

Don't fret, however! There is an easy way to do so, using Hugo's built-in server. This is the preferred method as it will automatically build and reload any changes you have made after spinning up the server. Run the following command to start the server:

``` bash
$ hugo server
```

### Adding New Event

To create a new event, you must create an event yaml file in `data/projects/` directory. Here's an example of an event yaml file:

```yaml
modalID: 5
title: Welfare Pack Giveaway
date: 2017-11-15
img: ay17181-welfare-pack.jpg
preview: ay17181-welfare-pack.jpg
category: Events
description: |

  1. Fill up NUSSU survey @ [bit.ly/ewp1718sem1](http://bit.ly/ewp1718sem1/)
  2. Fill up our survey @ [tiny.cc/SOCEWP1](http://tiny.cc/SOCEWP1/)
  3. Show us the confirmation email
  4. Collect your welfare pack @ Student Lounge
  
  Let's all do our best in our final lap in this semester! #EWPgiveaway
```

You must do the following:
1. Increment the `modalID`.
2. Change the title accordingly.
3. Place the event poster in `static/img/events/` and set the `img` and `preview` to the poster's filename. 
4. Change the description accordingly. You can use markdown to format the description.
5. Submit a pull request to the repository.


### Testing

As Hugo is a static website generator, there are currently no automated test suites. You can use `hugo server` to serve the site and test it with your favourite browser.

### Building

Once you are satisfied with the results, you can build the static website using the following command:

``` bash
$ hugo
```

The result will be placed in the `docs/` directory.

### Serving

This repository is set up to serve all files in the `docs/` directory publicly. To deploy any changes, simply push back to this repository. 
