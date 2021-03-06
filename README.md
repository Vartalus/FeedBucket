# FeedBasket

## What it does

A simple rss tool which uses bookmarks to save feeds and browsing history to track read/unread feed items.

## Live Version

See here for the live version: https://addons.mozilla.org/en-US/firefox/addon/feedbasket/

## Required installations

Make sure you have [NodeJS][nodejs] installed along with [Python2][python2]. This was last tested using NodeJS 12.14.1 and Python 2.7.17. If you use later versions of these apps, the package.json devDependencies may need updating, especially node-sass.

## Usage

First, you need to install all
[NodeJS][nodejs] dependencies with [npm](http://npmjs.com/) or
[yarn](https://yarnpkg.com/):

    npm install

Start the continuous build process to transpile the code into something that
can run in Firefox or Chrome:

    npm run build

This creates a WebExtension in the `extension` subdirectory.
Any time you edit a file, it will be rebuilt automatically.

In another shell window, run the extension in Firefox using a wrapper
around [web-ext][web-ext]:

    npm start

Any time you edit a file, [web-ext][web-ext] will reload the extension
in Firefox. To see the popup, click the icon from the browser bar.
Here is what it looks like:

![FeedBasket screenshot](screenshots/feedbasket.png "FeedBasket screenshot")

[react]: https://facebook.github.io/react/
[nodejs]: https://nodejs.org/en/
[web-ext]: https://developer.mozilla.org/en-US/Add-ons/WebExtensions/Getting_started_with_web-ext
[python2]: https://www.python.org/downloads/windows/
