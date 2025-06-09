# palette.game.web

> View our article on [Web Requests]($pedia/web-requests/) for an explanation of these blocks.

# show-browser -- Open URL in Browser

Opens the given URL in the system's default web browser. On mobile devices, this will open up the browser app. To view pages in-game, use the [Web Views](https://community.stencyl.com/index.php/topic,26708.0.html) extension.

> For a Flash game you may need to give [permissions]($pedia/web-flash-security/) to access the web.

# visit-site -- GET Request

Issues an HTTP GET request at the given URL, then executes the enclosed blocks if the request succeeded. The server's response is enclosed in the `site's response` block.

> For a Flash game you may need to give [permissions]($pedia/web-flash-security/) to access the web.

# visit-site-post -- POST Request

Issues an HTTP POST request at the given URL with the given parameters, then executes the enclosed blocks if the request succeeded. The server's response is enclosed in the `site's response` block.

Parameters are pased in as key=value pairs, separated by ampersands (&), like this `name=John&id=123456`.

> For a Flash game you may need to give [permissions]($pedia/web-flash-security/) to access the web.