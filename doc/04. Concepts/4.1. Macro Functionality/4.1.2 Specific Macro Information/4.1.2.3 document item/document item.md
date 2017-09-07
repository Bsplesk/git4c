## Specific macro information

### Get specific document item
Git4C backend allows you to request specific document item from repository defined in macro. Result of this request contains many information about file and  it's content.

```
POST {git4c-backend-url}/{uuid}/doc-item
```

##### Example request and response
```
Request URL:
    http://naatlas-confluence.openstack.local:8090/rest/doc/1.0/documentation/13e022d6cb1442c9ab7c8148bbd9c090/doc-item


Request Method:
    POST

Request Headers:
    POST /rest/doc/1.0/documentation/13e022d6cb1442c9ab7c8148bbd9c090/doc-item HTTP/1.1
    Host: naatlas-confluence.openstack.local:8090
    Connection: keep-alive
    Content-Length: 59
    Accept: application/json, text/plain, */*
    Origin: http://naatlas-confluence.openstack.local:8090
    X-Requested-With: XMLHttpRequest
    User-Agent: Mozilla/5.0 (Windows NT 6.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/60.0.3112.113 Safari/537.36
    Content-Type: application/json;charset=UTF-8
    Referer: http://naatlas-confluence.openstack.local:8090/display/TS/Markup-test
    Accept-Encoding: gzip, deflate
    Accept-Language: pl-PL,pl;q=0.8,en-US;q=0.6,en;q=0.4
    Cookie: JSESSIONID=13F1F830FE60CA13C502A0A3A326293B

Request Payload:
{
    "file": "modules/meps/src/main/resources/wsdl/generate.md"
}

Response Status Code:
    200 OK

Response Body:
{
   "uuid": "modules/meps/src/main/resources/wsdl/generate.md",
   "fullName": "modules/meps/src/main/resources/wsdl/generate.md",
   "name": "generate.md",
   "locationPath":[
        "modules",
        "meps",
        "src",
        "main",
        "resources",
        "wsdl",
        "generate.md"
   ],
   "lastUpdateAuthorName": "tkubicz",
   "lastUpdateAuthorEmail": "tkubicz@networkedassets.org",
   "lastUpdateTime":1492008922000,
   "content": "<span><h3 name=\"6beede81a2a04b5999e49e8fc418e2a0\">How to generate java classes from WSDL</h3> \n<p>To generate classes use 'wsimport' tool use command below:</p> \n<pre><code class=\"language-sh git4c-code git4c-highlightjs-code\">wsimport ProvisioningService.wsdl -p \"de.kdg.vas.nps.fixedip.core.provisioning\" -encoding \"UTF-8\" -keep\n</code></pre></span>",
   "rawContent": "### How to generate java classes from WSDL\n\nTo generate classes use 'wsimport' tool use command below:\n\n```sh\nwsimport ProvisioningService.wsdl -p \"de.kdg.vas.nps.fixedip.core.provisioning\" -encoding \"UTF-8\" -keep\n```",
   "tableOfContents":{
        "name": "",
        "anchorName": "",
        "children":[{
            "name": "How to generate java classes from WSDL",
            "anchorName": "6beede81a2a04b5999e49e8fc418e2a0",
            "children":[]
         }]
   }
}
```
