
Given Request param "{name}" is "{value}"
=============================================================================================================

Usage example
-------------

```
Feature: zato-apitest docs

Scenario: Given Request param "{name}" is "{value}"

    Given address "http://apitest-demo.zato.io"
    Given URL path "/demo/post"
    Given HTTP method "POST"
    Given format "FORM"
    Given Request param "key1" is "value1"
    Given Request param "key2" is "value2"

    When the URL is invoked

    Then status is "200"
```

Discussion
----------

This will send the request with http header 
Content-Type: application/x-www-form-urlencoded

