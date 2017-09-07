
### Get file

Endpoint for getting a file from predefined repository is available at:

```
POST {git4c-backend-url}/predefine/{uuid}/file
```


The payload of the request should be a JSON with specifiaction of a file and the branch.

Backend classes containing information about file and branch are defined as follows:

```
data class RequestedFile(
        val file: String
)

data class Branch(
    val branch: String
)
```


#### Example request and response
```
Request URL:
    http://pc-kurban:1990/confluence/rest/doc/1.0/documentation/predefine/e48d4c85c7ce470d91500b2f7ce1b2b9/file


Request Method:
    POST

Request Payload:
{
    "branch": "master",
    "file": "confluence-plugin/LICENCE.md"
}


Request Headers:
    POST /confluence/rest/doc/1.0/documentation/predefine/e48d4c85c7ce470d91500b2f7ce1b2b9/file HTTP/1.1
    Host: pc-kurban:1990
    Connection: keep-alive
    Content-Length: 57
    Accept: application/json, text/plain, */*
    Origin: http://pc-kurban:1990
    X-Requested-With: XMLHttpRequest
    User-Agent: Mozilla/5.0 (Windows NT 6.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/60.0.3112.113 Safari/537.36
    Content-Type: application/json;charset=UTF-8
    Referer: http://pc-kurban:1990/confluence/pages/createpage.action?spaceKey=ds
    Accept-Encoding: gzip, deflate
    Accept-Language: pl-PL,pl;q=0.8,en-US;q=0.6,en;q=0.4
    Cookie: JSESSIONID=AE443C4BAB5989773D070B4AAB512FF7; confluence.browse.space.cookie=space-templates

Response Status Code:
    200 OK

Response Body:
{
    "content": "<p> file content </p>"
}
```