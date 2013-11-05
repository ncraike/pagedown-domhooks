pagedown-domhooks
=================

Plugin for Markdown implementation [Pagedown](https://github.com/ncraike/pagedown-domhooks) which lets other plugins manipulate the final HTML using a DOM (Document Object Model).

This is intended to just support other plugins, such as [pagedown-toc](https://github.com/ncraike/pagedown-toc) (a table-of-contents generating plugin) which are most easily implemented using DOM selectors to query the structure of the final HTML.

Initially this is just targeting server-side environments for Pagedown, primarily node.js, using [jsdom]() to provide the DOM implementation. However, it should be possible to support the web browser environment in the future, hopefully exposing the browser's own DOM in an agnostic way, so plugins don't particularly have to care whether they're running server-side or in a browser.
