# SearXNG-Web-Extension (Unofficial)
<p align="center">
  <a href="https://addons.mozilla.org/en-US/firefox/addon/searxng-search"><img src="https://img.shields.io/amo/users/searxng-search?style=flat-square" alt="Badge" /></a>
</p>

**SearXNG** is a free Internet metasearch engine that aggregates results from various search services and databases. Users are not tracked or profiled.

[**SearXNG**](https://github.com/searxng/searxng) is a fork of [**SearX**](https://github.com/searx/searx).

[**Original SearXNG repository on GitHub**](https://github.com/searxng/searxng).

[**SearXNG instances**](https://searx.space/) - you can use other instances of the SearXNG search engine (for this you will need to fork the repository and replace the link for the search query in `manifest.json`).

# How does it work?
Extension use `manifest.json` settings which change your main search engine.

Example:

(**Default settings**)
```json
{
  "chrome_settings_overrides": {
    "search_provider": {
      "search_url": "https://example.com/search?q={searchTerms}"
    }
  }
}
```

(**With addon**)
```json
{
  "chrome_settings_overrides": {
    "search_provider": {
      "search_url": "https://searx.be/search?q={searchTerms}"
    }
  }
}
```

It means that your browser starts to use second link when you make search request.

# Tricks
If you want use **SearXNG** as support to main search engine do this:
- fork this repository and change the search URL according to your domain
- add this addon into your browser
- agree when browser shows you "Add this extension?"
- disagree when browser shows "Do you want change your main search engine?"
- use keywords like `@searxng, @searx, @sx` if you want use **SearXNG** when you make request

# Contributors
[**Erghel**](https://github.com/Erghel) - main contributor.
[**Rodion Borisov**](https://github.com/vintprox) - found `"suggestion_url"` and etc.  
[**Ivan Muzyka**](https://github.com/SeryiBaran) - found icons and etc.
