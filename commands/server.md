# wp server

Launch PHP's built-in web server for this specific WordPress installation.

Uses `php -S` to launch a web server serving the WordPress webroot.
&lt;http://php.net/manual/en/features.commandline.webserver.php&gt;

### OPTIONS

[\--host=&lt;host&gt;]
: The hostname to bind the server to.
\---
default: localhost
\---

[\--port=&lt;port&gt;]
: The port number to bind the server to.
\---
default: 8080
\---

[\--docroot=&lt;path&gt;]
: The path to use as the document root. If the path global parameter is
set, the default value is it.

[\--config=&lt;file&gt;]
: Configure the server with a specific .ini file.

### EXAMPLES

    # Make the instance available on any address (with port 8080)
    $ wp server --host=0.0.0.0
    PHP 5.6.9 Development Server started at Tue May 24 01:27:11 2016
    Listening on http://0.0.0.0:8080
    Document root is /
    Press Ctrl-C to quit.

    # Run on port 80 (for multisite)
    $ sudo wp server --host=localhost.localdomain --port=80
    PHP 5.6.9 Development Server started at Tue May 24 01:30:06 2016
    Listening on http://localhost1.localdomain1:8080
    Document root is /
    Press Ctrl-C to quit.

    # Configure the server with a specific .ini file
    $ wp server --config=development.ini
    PHP 7.0.9 Development Server started at Mon Aug 22 12:09:04 2016
    Listening on http://localhost:8080
    Document root is /
    Press Ctrl-C to quit.


