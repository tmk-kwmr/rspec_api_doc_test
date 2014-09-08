# Orders API

## PUT /orders/:id

### PUT /orders/:id

### Parameters

Name : name
Description : Name of order

Name : paid
Description : If the order has been paid for

Name : email
Description : Email of user that placed the order

### Request

#### Headers

<pre>Accept: application/json
Content-Type: application/json
Host: example.org
Cookie: </pre>

#### Route

<pre>PUT /orders/1</pre>

#### Body

<pre>{"order":{"name":"Updated Name"}}</pre>

#### cURL

<pre class="request">curl &quot;http://localhost:3000/orders/1&quot; -d &#39;{&quot;order&quot;:{&quot;name&quot;:&quot;Updated Name&quot;}}&#39; -X PUT \
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
X-Request-Id: f0506350-fcba-4a50-8925-e49457351a53
X-Runtime: 0.003955</pre>

#### Status

<pre>204 No Content</pre>

