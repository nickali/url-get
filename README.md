
# Expand or Unshorten URLs

This scrapes [urlex.org](https://urlex.org) to get the final URL of a passed in URL. 

The use case is getting the final URL of tracked links in email, especially if you are using an ad blocker that filters by domain. For example, you have a link like "https://e.customeriomail.com/e/c/..." but you have blocked customeriomail.com.

# Usage

```shell
python url-get.py <URL>
```

To build a binary, install my pyinstaller and then run

```shell
pyinstaller --onefile url-get.py
```

Put the dist/url-get somewhere your path references and make it executable.

URL can be encoded or not.

# Don't abuse it

urlex.org allows for 100 checks per day. If you are going to use them more, sign up for their Pro plan and use the API properly instead of this.

**Seriously, don't be a dick.**
