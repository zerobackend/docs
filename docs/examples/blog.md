

Here is an example of simple `blog` configuration entity files

# Post

```
{
  "label": "Post",
  "name": "post",
  "fields": [
    {
      "label": "Title",
      "name": "title",
      "dataType": "string",
      "displayType": {
        "list": "string",
        "show": "string",
        "create": "string",
        "edit": "string"
      }
    },
    {
      "label": "Source URL",
      "name": "source_url",
      "dataType": "string",
      "displayType": {
        "list": "none",
        "show": "string",
        "create": "string",
        "edit": "string"
      }
    },
    {
      "label": "Short description",
      "name": "description",
      "dataType": "string",
      "displayType": {
        "list": "none",
        "show": "text",
        "create": "text",
        "edit": "text"
      }
    },
    {
      "label": "Content",
      "name": "content",
      "dataType": "string",
      "displayType": {
        "list": "none",
        "show": "html",
        "create": "text",
        "edit": "text"
      }
    },
    {
      "label": "Publish date",
      "name": "published_at",
      "dataType": "date",
      "displayType": {
        "list": "none",
        "show": "date",
        "create": "date",
        "edit": "date"
      }
    },
    {
      "label": "Categories",
      "name": "categories",
      "dataType": "reference_many",
      "dataRefName": "post_x_category",
      "dataRefEntity": "category",
      "dataRefField": "label",
      "displayType": {
        "list": "none",
        "show": "string",
        "create": "string",
        "edit": "string"
      }
    },
    {
      "label": "Tags",
      "name": "tags",
      "dataType": "reference_many",
      "dataRefName": "post_x_tag",
      "dataRefEntity": "tag",
      "dataRefField": "label",
      "displayType": {
        "list": "none",
        "show": "string",
        "create": "string",
        "edit": "string"
      }
    },
    {
      "label": "Cover",
      "name": "cover_image_url",
      "dataType": "string",
      "displayType": {
        "list": "none",
        "show": "string",
        "create": "string",
        "edit": "string"
      }
    },
    {
      "label": "Vimeo URL",
      "name": "cover_vimeo_url",
      "dataType": "string",
      "displayType": {
        "list": "none",
        "show": "string",
        "create": "string",
        "edit": "string"
      }
    },
    {
      "label": "Youtube URL",
      "name": "cover_youtube_url",
      "dataType": "string",
      "displayType": {
        "list": "none",
        "show": "string",
        "create": "string",
        "edit": "string"
      }
    }
  ]
}
```


# Category

```
{
  "label": "Category",
  "name": "category",
  "fields": [
    {
      "label": "Category title",
      "name": "title",
      "dataType": "string",
      "displayType": {
        "list": "string",
        "show": "string",
        "create": "string",
        "edit": "string"
      }
    },
    {
      "label": "Posts",
      "name": "posts",

      "dataType": "reference_many",
      "dataRefName": "post_x_category",
      "dataRefEntity": "post",
      "dataRefField": "title",
      
      "displayType": {
        "list": "none",
        "show": "string",
        "create": "string",
        "edit": "string"
      }
    }
  ]
}
```



# Tag

```
{
  "label": "Tag",
  "name": "tag",
  "fields": [
    {
      "label": "Tag",
      "name": "title",
      "dataType": "string",
      "displayType": {
        "list": "string",
        "show": "string",
        "create": "string",
        "edit": "string"
      }
    },
    {
      "label": "Posts",
      "name": "posts",

      "dataType": "reference_many",
      "dataRefName": "post_x_tag",
      "dataRefEntity": "post",
      "dataRefField": "title",
      
      "displayType": {
        "list": "none",
        "show": "string",
        "create": "string",
        "edit": "string"
      }
    }
  ]
}
```



