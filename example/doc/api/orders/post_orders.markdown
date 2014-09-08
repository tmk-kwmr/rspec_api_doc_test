# Orders API

## POST /orders

### POST /orders

First, create an order, then make a later request to get it back

### Parameters

Name : name *- required -*
Description : Name of order

Name : paid *- required -*
Description : If the order has been paid for

Name : email
Description : Email of user that placed the order


### Response Fields

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

<pre>POST /orders</pre>

#### Body

<pre>{"order":{"name":"Order 1","paid":true,"email":"email@example.com"}}</pre>

#### cURL

<pre class="request">curl &quot;http://localhost:3000/orders&quot; -d &#39;{&quot;order&quot;:{&quot;name&quot;:&quot;Order 1&quot;,&quot;paid&quot;:true,&quot;email&quot;:&quot;email@example.com&quot;}}&#39; -X POST \
	-H &quot;Accept: application/json&quot; \
	-H &quot;Content-Type: application/json&quot; \
	-H &quot;Host: example.org&quot; \
	-H &quot;Cookie: &quot;</pre>

### Response

#### Headers

<pre>X-Frame-Options: SAMEORIGIN
X-XSS-Protection: 1; mode=block
X-Content-Type-Options: nosniff
Location: http://example.org/orders/1
Content-Type: application/json; charset=utf-8
ETag: &quot;5c0e2693e8c687d2a67861f42f3b886c&quot;
Cache-Control: max-age=0, private, must-revalidate
X-Request-Id: 7cdb7328-8eea-44ed-a4a1-d777947e308b
X-Runtime: 0.004846
Content-Length: 145</pre>

#### Status

<pre>201 Created</pre>

#### Body

<pre>{"id":1,"name":"Order 1","paid":true,"email":"email@example.com","created_at":"2014-09-08T09:23:19.529Z","updated_at":"2014-09-08T09:23:19.529Z"}</pre>
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
ETag: &quot;5c0e2693e8c687d2a67861f42f3b886c&quot;
Cache-Control: max-age=0, private, must-revalidate
X-Request-Id: 3a8f7c72-0e02-472a-932a-a6e69199ad76
X-Runtime: 0.002272
Content-Length: 145</pre>

#### Status

<pre>200 OK</pre>

#### Body

<pre>{"id":1,"name":"Order 1","paid":true,"email":"email@example.com","created_at":"2014-09-08T09:23:19.529Z","updated_at":"2014-09-08T09:23:19.529Z"}</pre>
