# jkotzker.dev

Redirects every path on `jkotzker.dev` to the same path on `https://josephkotzker.com`. GitHub Pages cannot send a server-side 301, so `index.html` and `404.html` redirect client-side (`location.replace`, with a meta refresh fallback). The site itself lives in `jkotzker/josephkotzker.com`.

Clients without JavaScript follow the meta refresh and land on the home page rather than the same path. Paths other than `/` are served from `404.html` with HTTP status 404, which is what lets the script see the requested path.
