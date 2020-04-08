# CORSJavascriptExample
## Javascript Example With CORS

This is a simple call to the Ungerboeck API that shows you how to use Javascript with AJAX.  It also gives an example on how CORS works within an API call.

To enable CORS, you can run the web configuration utility.  The Ungerboeck API tab will have a checkbox to enable cors, along with an Allowed Origin URL white list field.
		
You can also directly modify the web.config file.

```xml
<appSettings>
    <add key="AllowCORS" value="Y" />
    <add key="CORSAllowedOriginURLs" value="https://[originalsitedomain]" />
</appSettings>

<security>
  <requestFiltering allowDoubleEscaping="true">
     <verbs>
        <add verb="OPTIONS" allowed="True" />
      </verbs>
   </requestFiltering>
</security>
```

For the full instructions, check out our [knowledgebase article](https://supportcenter.ungerboeck.com/hc/en-us/articles/360046108533-Ungerboeck-API-and-CORS)