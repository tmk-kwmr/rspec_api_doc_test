# Orders API

## Getting the headers

### HEAD /orders
### Request

#### Headers

<pre>Accept: application/json
Content-Type: application/json
Host: example.org
Cookie: </pre>

#### Route

<pre>HEAD /orders</pre>

#### cURL

<pre class="request">curl &quot;http://localhost:3000/orders&quot; -X HEAD \
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
X-Request-Id: 8cef7842-1c23-471e-9d03-226384972b75
X-Runtime: 0.001596</pre>

#### Status

<pre>204 No Content</pre>

