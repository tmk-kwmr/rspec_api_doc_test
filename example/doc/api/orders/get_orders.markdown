# Orders API

## GET /orders

### GET /orders

### Parameters

Name : page
Description : orders一覧

### Request

#### Headers

<pre>Accept: application/json
Content-Type: application/json
Host: example.org
Cookie: </pre>

#### Route

<pre>GET /orders?page=1</pre>

#### Query Parameters

<pre>page: 1</pre>

#### cURL

<pre class="request">curl &quot;http://localhost:3000/orders?page=1&quot; -X GET \
	-H &quot;Accept: application/json&quot; \
	-H &quot;Content-Type: application/json&quot; \
	-H &quot;Host: example.org&quot; \
	-H &quot;Cookie: &quot;</pre>

### Response

#### Headers

<pre>X-Frame-Options: SAMEORIGIN
X-XSS-Protection: 1; mode=block
X-Content-Type-Options: nosniff
Content-Type: application/json; charset=utf-8
ETag: &quot;8d9c6be1b1894c345961d33f8c838cd7&quot;
Cache-Control: max-age=0, private, must-revalidate
X-Request-Id: a412abe6-ba37-4827-8cb2-3efeb36fc373
X-Runtime: 0.002944
Content-Length: 295</pre>

#### Status

<pre>200 OK</pre>

#### Body

<pre>[{"id":1,"name":"Order 0","paid":true,"email":"email0@example.com","created_at":"2014-09-08T09:23:19.501Z","updated_at":"2014-09-08T09:23:19.501Z"},{"id":2,"name":"Order 1","paid":true,"email":"email1@example.com","created_at":"2014-09-08T09:23:19.502Z","updated_at":"2014-09-08T09:23:19.502Z"}]</pre>
