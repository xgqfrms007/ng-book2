# what is gitbook metadata ?


https://www.gitbook.com/book/centerforgov/open-data-metadata-guide/details  




https://www.npmjs.com/package/gitbook-plugin-meta  

## gitbook.json
```json
{
    "plugins": [
        "meta"
    ],
    "pluginsConfig": {
        "meta": {
            "name": "apple-mobile-web-app-capable",
            "content": "yes"
        }
    }
}
``` 

> equal to

```html
<meta name="apple-mobile-web-app-capable" content="yes">
``` 
> in the <head> section of your book.  

If you have **multiple metadata** to add, then you can:  

```json
{
    "plugins": [
        "meta"
    ],
    "pluginsConfig": {
        "meta": {
            "data": [
                {
                    "name": "name1",
                    "content": "content1",
                    "extra": "Any information"
                },
                {
                    "name": "name2",
                    "content": "content2"
                },
            ]
        }
    }
}
``` 


> equal to

```html
<meta name="apple-mobile-web-app-capable" content="yes">
<meta name="apple-mobile-web-app-capable" content="yes">
``` 
> in the <head> section of your book.  ???

## demo codes  

https://github.com/CyberZHG/CLRS/edit/master/book.json  

```json
{
    "plugins": [
        "scrollablecode",
        "fancybox",
        "disqus",
        "github",
        "search",
        "ga",
        "mathjax",
        "meta",
        "sitemap-general"
    ],
    "pluginsConfig": {
        "disqus": {
            "shortName": "clrs",
            "useIdentifier": false
        },
        "github": {
            "url": "https://github.com/CyberZHG/CLRS"
        },
        "ga": {
            "token": "UA-75597402-1",
            "configuration": "auto"
        },
        "meta": {
            "name": "google-site-verification",
            "content": "AJ-kdEF3EADDcL_4CuIJs3V29ZkarsZBX-YmVZ3FCeA"
        },
        "sitemap-general": {
            "prefix": "https://cyberzhg.gitbooks.io/clrs/content/"
        }
    }
}

``` 











