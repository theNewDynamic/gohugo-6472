# gohugo-6472

This is an example repo for [gohugoio/hugo/issues/6472](https://github.com/gohugoio/hugo/issues/6472)

## Step to reproduce

Run `hugo --minify`

Even though the error message points to an HTML file:
```
Error: Error building site: failed to render pages: parse error:1:1: unexpected character
    1: <!DOCTYPE html><html><head><title>http://example.org/arti...
```

Removing the JSON output from `content/article/_index.md` Front Matter removes the error.