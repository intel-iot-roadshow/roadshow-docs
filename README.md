# Getting Started Guides

These guides are used at Intel IoT Roadshows.

## Contributing

We welcome pull requests and bug reports on these docs. Please read the [Intel® IoT Getting Started Docs Contribution Guide](CONTRIBUTING.md) for more information.

## Branches

### branch: master

[github.com/intel-iot-roadshow/getting-started-guides](https://github.com/intel-iot-roadshow/getting-started-guides)

This is the [Jekyll](http://jekyllrb.com/) templating source code to produce the static html files for both the 'gh-pages' and 'html' branches.

Make changes to this branch only. If you try updating 'html' or 'gh-pages', your changes **will** be overwritten.

### branch: html

[github.com/intel-iot-roadshow/getting-started-guides/tree/html](https://github.com/intel-iot-roadshow/getting-started-guides/tree/html)

**THIS IS THE BRANCH THAT CAN BE DOWNLOADED AND PUT ON USB KEYS FOR ROADSHOWS.** 

Static files need to be generated form the 'jekyll' branch. See [the branch's README](https://github.com/intel-iot-roadshow/getting-started-guides/blob/html/README.md) for details on running a local web server to view files.

### branch: gh-pages

[github.com/intel-iot-roadshow/getting-started-guides/tree/gh-pages](https://github.com/intel-iot-roadshow/getting-started-guides/tree/gh-pages)

Github's built in web server for viewing html files: [intel-iot-roadshow.github.io/getting-started-guides/](http://intel-iot-roadshow.github.io/getting-started-guides/). Feel free to send anyone to this url if they are unable to get the USB key files working. Static files need to be generated form the 'jekyll' branch.

## Installation

You will need to have Jekyll (and Ruby) installed to preview the site on your computer and to build the static html files.

```
gem install jekyll
```

## Previewing site locally

Run the following command, then visit http://localhost:4000/.

```
jekyll serve
```

Alternatively:

```
bundle exec jekyll serve
```


## Building static html files

```
jekyll build
```

Generated files end up in a folder named `_site`. Copy the contents of _site in order to commit new files to the 'html' branch.


## Building static html files for gh-pages

```
jekyll build --config _config.gh-pages.yml
```

The extra flag uses a config file that includes "/getting-started-guides" (which is the name of this Github repo) as a base url instead of "" or "/" in order to make it compatible when viewing on the github.io domain.

Generated files end up in the `_site` folder too. Copy the contents of _site in order to commit new files to the 'gh-pages' branch. Once commits have been pushed to 'gh-pages', the docs can be viewed at [intel-iot-roadshow.github.io/getting-started-guides/](http://intel-iot-roadshow.github.io/getting-started-guides/)
