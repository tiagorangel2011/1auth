1auth
=====

1auth is a very simple to use auth service built thinking of [privacy](/pp.html)

* * *

Using 1auth
===========

There are 3 ways of using 1auth:

*   redirect your user to `https://1auth.glitch.me/auth?redirect=_[REDIRECTION_URL]_&name=_[YOUR_APP_NAME]_&logo=_[LOGO_URL]_` (Replace `[LOGO_URL]` with a `60x60px _SVG/GIF/PNG/JPG/JPEG_` logo URL)

*   **(don't do this)** Use a `window.open()` popup

*   **(recommended)** Use our library:
    

We recommend you to use our [setup wizard](https://1auth.glitch.me/wizard.html) to get started.

When logged in, 1auth will redirect you to `_[REDIRECTION_URL]_` and send the JSON response from Google as the URL `GET` query "response". Here is an example JSON response:

In the response URI, you will need to `URI` decode the response, like this:

After gotting a response, we recommend you storing the JSON as a cookie/local storage so the user does not need to sign up every time a new page opens.

* * *

Examples
========

*   [Open in the current tab](https://1auth.glitch.me/auth?redirect=/response.html&name=Sample app&logo=https://google.com/favicon.ico)

* * *

Troubleshooting
===============

If you are having a error, look for the error ID and check the resolution here.

#### ERR\_MISSING\_QUERY

One or more required URL queries are missing. Check the URL

#### ERR\_ACTV\_JAVASCRIPT

The client needs to enable JS

* * *

[1auth](https://1auth.glitch.me/) by [Tiago Rangel de Sousa](https://tiagorangel.com) is licensed under [CC BY-ND 4.0![](https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1)![](https://mirrors.creativecommons.org/presskit/icons/by.svg?ref=chooser-v1)![](https://mirrors.creativecommons.org/presskit/icons/nd.svg?ref=chooser-v1)](http://creativecommons.org/licenses/by-nd/4.0/?ref=chooser-v1)

The code is open-sourced at [Glitch](https://glitch.com/edit/#!/1auth?utm-source=github-md)
