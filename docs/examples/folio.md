
Here is an example of simple `folio` configuration entity files

# Project

```
{
  "label": "Project",
  "name": "project",
  "fields": [
    {
      "label": "Project title",
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
      "label": "Website",
      "name": "website",
      "dataType": "string",
      "displayType": {
        "list": "none",
        "show": "string",
        "create": "string",
        "edit": "string"
      }
    },
    {
      "label": "Client",
      "name": "client",
      "dataType": "string",
      "displayType": {
        "list": "string",
        "show": "string",
        "create": "string",
        "edit": "string"
      }
    },
    {
      "label": "Description",
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
      "label": "Project release date",
      "name": "release_date",
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
      "dataRefName": "project_x_category",
      "dataRefEntity": "category",
      "dataRefField": "title",

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
      "dataRefName": "project_x_tag",
      "dataRefEntity": "tag",
      "dataRefField": "title",

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
      "label": "Projects",
      "name": "projects",

      "dataType": "reference_many",
      "dataRefName": "project_x_category",
      "dataRefEntity": "project",
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
      "label": "Projects",
      "name": "projects",

      "dataType": "reference_many",
      "dataRefName": "project_x_tag",
      "dataRefEntity": "project",
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



