# Orders API

## GET /orders/:id

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
ETag: &quot;f7dea916698fd23f02cce80b0800e3fd&quot;
Cache-Control: max-age=0, private, must-revalidate
X-Request-Id: 1f05ffad-3362-4fba-b1c9-466161bf64b9
X-Runtime: 0.012819
Content-Length: 146</pre>

#### Status

<pre>200 OK</pre>

#### Body

<pre>{"id":1,"name":"Old Name","paid":true,"email":"email@example.com","created_at":"2014-09-08T09:23:19.475Z","updated_at":"2014-09-08T09:23:19.475Z"}</pre>
