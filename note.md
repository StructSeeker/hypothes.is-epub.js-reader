# Modify Title

```
let iframe = document.querySelector('.epub-view > iframe')
let iframedoc = iframe.contentWindow.document

iframe.onload = () => {
    iframedoc.querySelector('title').prepend(document.querySelector('title').innerHTML);
}

```

# Require Cors for bookPath

# Use bookPath treated as folder 

https://github.com/futurepress/epub.js/issues/1320


# Fix security flaw:
Remove iframe's allow-same-origin, allow-script, add enable-annotation
Wait for epub.js 0.4

# Try form

 <input type="text" id="name" name="name"/>