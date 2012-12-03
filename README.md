browserstack-cli
================

A command line interface for the browserstack api.

```
Usage: browserstack [options] [command]

  Commands:

    launch <browser> <url> Launch remote browser:version at a url. e.g. browserstack launch firefox:3.6 http://google.com
    kill <id>              Kill a running browser. An id of "all" will kill all running browsers
    list                   List running browsers
    browsers               List available browsers and versions
    tunnel <host:port>     Create a browserstack tunnel
    *

  Options:

    -h, --help                  output usage information
    -V, --version               output the version number
    -u, --user <user:password>  Browserstack authentication
    --os                        The os of the browser or device. Defaults to win.
    -t, --timeout <seconds>     Launch duration after which browsers exit
    --attach                    Attach process to remote browser.
    -k, --key                   Tunnling key.
    --ssl                       ssl flag for tunnel.
```

## ```~/.browserstack.json```

You can configure your browserstack username, password, and tunnel key in the file ```~/.browserstack.json``` like this:

```json
{
  "key": "XXXXXXXXXXXXXXXX",
  "username": "XXXXXXX",
  "password": "XXXXXXX"
}
```

## Your Browserstack Tunnel Key
If you're doing automated testing, use the key from the [automated browser testing page](http://www.browserstack.com/automated-browser-testing-api).

If you're launching browsers manually from the browserstack.com website, use the key from [this page](http://www.browserstack.com/local-testing#cmd-tunnel).
