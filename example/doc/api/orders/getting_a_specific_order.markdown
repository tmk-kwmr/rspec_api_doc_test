# Orders API

## Getting a specific order

### GET /orders/:id
### Request

#### Headers

<pre>Accept: application/json
Content-Type: application/json
Host: example.org
Cookie: </pre>

#### Route

<pre>GET /orders/1</pre>

#### cURL

<pre class="request">curl &quot;http://localhost:3000/orders/1&quot; -X GET \
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
ETag: &quot;7da2633d1386884f0d1a00a2ef751030&quot;
Cache-Control: max-age=0, private, must-revalidate
X-Request-Id: b5083b17-ad95-4e9e-8fcf-9bddc03b2399
X-Runtime: 0.002961
Content-Length: 146</pre>

#### Status

<pre>200 OK</pre>

#### Body

<pre>{"id":1,"name":"Old Name","paid":true,"email":"email@example.com","created_at":"2014-09-08T08:45:27.246Z","updated_at":"2014-09-08T08:45:27.246Z"}</pre>
