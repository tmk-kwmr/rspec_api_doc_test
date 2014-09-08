# Orders API

## get_order_id

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
ETag: &quot;e9e19c4b125fcd47056e7abc3d8ebef3&quot;
Cache-Control: max-age=0, private, must-revalidate
X-Request-Id: 274b8183-1ef8-42f8-b52f-bb0e0a6e2aff
X-Runtime: 0.002083
Content-Length: 146</pre>

#### Status

<pre>200 OK</pre>

#### Body

<pre>{"id":1,"name":"Old Name","paid":true,"email":"email@example.com","created_at":"2014-09-08T09:19:40.179Z","updated_at":"2014-09-08T09:19:40.179Z"}</pre>
