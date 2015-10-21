# README #

### What this does ###

This python script was created to automate the process of posting craigslist ads while emulating a real user via the Selenium browser engine.  It has the ability to spin content in the post title and post body to allow for completely dynamic ads.

In this script's current state, you **WILL** have to modify the selections in the script for proper navigation to your posting area.  This will be fixed in future versions.

### How to use ###

Usage of this script is incredibly simple.

```
python /path/to/craigslist-poster/__main__.py "LoginEmail" "LoginPassword" "Contact Phone Number" "ContactName" "Post Title (Spin allowed)" "Zip Code" "/path/to/content.txt" int(TimeDelay)
```

Example:
```
python /craigslist-poster/__main__.py "example@demo.com" "password" "123-456-7890" "Mike" "This is an {example|test} {post|ad}" "12345" "/craigslist-poster/content.txt" 3
```

### Requirements ###

* BeautifulSoup4 (**pip install beautifulsoup4**)
* Selenium (**pip install selenium**)
* FireFox (Should be included with Selenium)
* PyVirtualDisplay (**pip install pyvirtualdisplay**)
* Spintax (**pip install spintax**)
* Python 2.7

### Contribution guidelines ###

* All code will be reviewed and approved by repository owner.
* All commits must describe what has been done.
    * If multiple changes per commit, describe what was done in the commit description.