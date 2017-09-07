Remove all macros
=============

Git4C backend provides you with an endpoint to remove all data. This will also delete every macro that has ever been created.
This endpoint will also remove all predefined repositories and globs. <b>All data will be cleaned.</b>

```
DELETE {git4c-backend-url}/
```

#### Example request and response
```
Request URL:
    http://naatlas-confluence.openstack.local:8090/rest/doc/1.0/documentation

Request Method:
    DELETE

Request Headers:
    DELETE /confluence/rest/doc/1.0/documentation HTTP/1.1
    Host: naatlas-confluence.openstack.local:8090
    Connection: keep-alive
    Content-Length: 148
    Accept: application/json, text/plain, */*
    Origin: http://naatlas-confluence.openstack.local:8090
    X-Requested-With: XMLHttpRequest
    User-Agent: Mozilla/5.0 (Windows NT 6.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/60.0.3112.113 Safari/537.36
    Content-Type: application/json;charset=UTF-8
    Referer: http://naatlas-confluence.openstack.local:8090/pages/resumedraft.action?draftId=8486914&draftShareId=e94d482a-8f77-460a-a139-a0bee40f8779
    Accept-Encoding: gzip, deflate
    Accept-Language: pl-PL,pl;q=0.8,en-US;q=0.6,en;q=0.4
    Cookie: JSESSIONID=13F1F830FE60CA13C502A0A3A326293B

Response Status Code:
    200 OK
```