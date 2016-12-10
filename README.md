# ng-book2

[https://www.gitbook.com/book/xgqfrms-github/ng-book2/details](https://www.gitbook.com/book/xgqfrms-github/ng-book2/details)


***********************************************************************************************************

[目录](/chapters/content.md)







***********************************************************************************************************

## disqus 集成 gitbook 

https://plugins.gitbook.com/plugin/disqus

```json
{
    "plugins": ["disqus"],
    "pluginsConfig": {
        "disqus": {
            "shortName": "XXXXXXX"
        }
    }
}
```


***********************************************************************************************************


# Disqus comments for GitBook

Preview

To use the Disqus plugin in your Gitbook project, add the disqus plugin to the book.json file, along with your shortname (you create a shortname for disqus by creating a new website on the disqus.com website)
```json
{
    "plugins": ["disqus"],
    "pluginsConfig": {
        "disqus": {
            "shortName": "XXXXXXX"
        }
    }
}
``` 
Disable it for a specific page

Using the YAML frontmatter, you can disable the Disqus comments thread for a specific page:
```yaml
---
disqus: false
---
``` 
# My Page without disqus
Use custom page identifiers

By default Disqus use the window URL as the main identifier when creating a thread. You can set a custom identifier in the YAML frontmatter of your page:
```yaml
---
disqus:
  identifier: "some-identifier"
---
 Configuration
Setting	Description	Type	Allowed values
shortName 
required	Website Shortname	String
-
useIdentifier	Use page identifier	Boolean
-
``` 
