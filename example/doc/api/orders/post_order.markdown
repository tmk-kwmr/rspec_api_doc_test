# Orders API

## post_order

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
ETag: &quot;2edbd738d82bfec0baf8cd568088c562&quot;
Cache-Control: max-age=0, private, must-revalidate
X-Request-Id: 9a10f58f-8a8a-4948-b4e6-db16b8b3f2cb
X-Runtime: 0.004720
Content-Length: 145</pre>

#### Status

<pre>201 Created</pre>

#### Body

<pre>{"id":1,"name":"Order 1","paid":true,"email":"email@example.com","created_at":"2014-09-08T09:19:40.159Z","updated_at":"2014-09-08T09:19:40.159Z"}</pre>
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
ETag: &quot;2edbd738d82bfec0baf8cd568088c562&quot;
Cache-Control: max-age=0, private, must-revalidate
X-Request-Id: 94657678-9353-47c0-94d6-c606b9323b89
X-Runtime: 0.004221
Content-Length: 145</pre>

#### Status

<pre>200 OK</pre>

#### Body

<pre>{"id":1,"name":"Order 1","paid":true,"email":"email@example.com","created_at":"2014-09-08T09:19:40.159Z","updated_at":"2014-09-08T09:19:40.159Z"}</pre>
