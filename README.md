# SearXNG-Web-Extension (Unofficial)
[<img src="./firefox-add-ons.png" title="Firefox Add-ons" width="auto" height="47" />](https://addons.mozilla.org/en-US/firefox/addon/searxng-search) <p><a href=""><img src="https://img.shields.io/amo/users/searxng-search?style=flat-square" alt="Badge" /></a></p>

# SearXNG

**SearXNG** is a free Internet metasearch engine that aggregates results from various search services and databases. Users are not tracked or profiled.

[**SearXNG**](https://github.com/searxng/searxng) is a fork of [**SearX**](https://github.com/searx/searx).

[**Original SearXNG repository on GitHub**](https://github.com/searxng/searxng).

[**SearXNG instances**](https://searx.space/) - you can use other instances of the SearXNG search engine (for this you will need to fork the repository and replace the link for the search query in `manifest.json`).

# How does extension work?
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

# Tricks with extension
If you want use **SearXNG** as support to main search engine do this:
1. add this addon into your browser
2. agree when browser shows you "Add this extension?"
3. disagree when browser shows "Do you want change your main search engine?"
4. use keywords like `@searxng, @searx, @sx` if you want use **SearXNG** when you make request

# Contributors
[**Erghel**](https://github.com/Erghel) - main contributor.

[**Rodion Borisov**](https://github.com/vintprox) - found `"suggestion_url"` and etc.  

[**Ivan Muzyka**](https://github.com/SeryiBaran) - found icons and etc.
