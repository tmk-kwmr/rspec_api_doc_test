# Orders API

## get_orders

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
ETag: &quot;f751ee8ce29d01df7ae28b209b3c8ac2&quot;
Cache-Control: max-age=0, private, must-revalidate
X-Request-Id: 0a4991c0-6482-4cd6-890a-c25892ac3ee0
X-Runtime: 0.014214
Content-Length: 295</pre>

#### Status

<pre>200 OK</pre>

#### Body

<pre>[{"id":1,"name":"Order 0","paid":true,"email":"email0@example.com","created_at":"2014-09-08T09:19:40.128Z","updated_at":"2014-09-08T09:19:40.128Z"},{"id":2,"name":"Order 1","paid":true,"email":"email1@example.com","created_at":"2014-09-08T09:19:40.131Z","updated_at":"2014-09-08T09:19:40.131Z"}]</pre>
