# Orders API

## Creating an order

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
ETag: &quot;f7e3e17af9aecd91b101ff93725e3298&quot;
Cache-Control: max-age=0, private, must-revalidate
X-Request-Id: bf827878-aceb-45b6-8b25-31344838bac4
X-Runtime: 0.004770
Content-Length: 145</pre>

#### Status

<pre>201 Created</pre>

#### Body

<pre>{"id":1,"name":"Order 1","paid":true,"email":"email@example.com","created_at":"2014-09-08T08:45:27.271Z","updated_at":"2014-09-08T08:45:27.271Z"}</pre>
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
ETag: &quot;f7e3e17af9aecd91b101ff93725e3298&quot;
Cache-Control: max-age=0, private, must-revalidate
X-Request-Id: ccc55c7c-a122-4a17-9119-936f9ec16182
X-Runtime: 0.001938
Content-Length: 145</pre>

#### Status

<pre>200 OK</pre>

#### Body

<pre>{"id":1,"name":"Order 1","paid":true,"email":"email@example.com","created_at":"2014-09-08T08:45:27.271Z","updated_at":"2014-09-08T08:45:27.271Z"}</pre>
