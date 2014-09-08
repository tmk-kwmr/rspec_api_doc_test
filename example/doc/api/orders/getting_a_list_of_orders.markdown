# Orders API

## Getting a list of orders

### GET /orders

### Parameters

Name : page
Description : Current page of orders

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
ETag: &quot;eaa72af26116acbdc5a277ce2d185d1d&quot;
Cache-Control: max-age=0, private, must-revalidate
X-Request-Id: 92bde99a-9951-45d2-8093-4fbdf8c440bc
X-Runtime: 0.002810
Content-Length: 295</pre>

#### Status

<pre>200 OK</pre>

#### Body

<pre>[{"id":1,"name":"Order 0","paid":true,"email":"email0@example.com","created_at":"2014-09-08T08:45:27.259Z","updated_at":"2014-09-08T08:45:27.259Z"},{"id":2,"name":"Order 1","paid":true,"email":"email1@example.com","created_at":"2014-09-08T08:45:27.260Z","updated_at":"2014-09-08T08:45:27.260Z"}]</pre>
