`FILES.md` -- not called `README.md` to make it harder to discover with random probes.

`index.html` -- empty, to hide the contents of this directory if it's placed under the document root of a webserver (also why no README.md). Probably a good idea to `sudo touch data.d/index.html` if it is under the document root somewhere.

`channel.vote.block` -- actual template used for the poll JSON block
`sample.vote.block` -- output from Slack's Block Kit Builder for the poll JSON block

`lunch` -- a Perl CGI script with taint checks (for security, don't disable), `use strict` / `use warnings` for better safety while coding (okay to disable), and a bunch of debug code, all (or most) of which will be found with `grep DEBUG`
