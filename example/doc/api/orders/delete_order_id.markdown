# Orders API

## delete_order_id

### DELETE /orders/:id
### Request

#### Headers

<pre>Accept: application/json
Content-Type: application/json
Host: example.org
Cookie: </pre>

#### Route

<pre>DELETE /orders/1</pre>

#### cURL

<pre class="request">curl &quot;http://localhost:3000/orders/1&quot; -d &#39;&#39; -X DELETE \
	-H &quot;Accept: application/json&quot; \
	-H &quot;Content-Type: application/json&quot; \
	-H &quot;Host: example.org&quot; \
	-H &quot;Cookie: &quot;</pre>

### Response

#### Headers

<pre>X-Frame-Options: SAMEORIGIN
X-XSS-Protection: 1; mode=block
X-Content-Type-Options: nosniff
Cache-Control: no-cache
X-Request-Id: 135a62e9-81fd-4c4a-9ec9-219e098f5836
X-Runtime: 0.002693</pre>

#### Status

<pre>204 No Content</pre>

