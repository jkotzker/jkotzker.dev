# jkotzker.dev

Redirects every path on `jkotzker.dev` to the same path on `https://josephkotzker.com`. GitHub Pages cannot send a server-side 301, so `index.html` and `404.html` redirect client-side (`location.replace`, with a meta refresh fallback). The site itself lives in `jkotzker/josephkotzker.com`.
