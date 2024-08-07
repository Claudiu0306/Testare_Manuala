<h1>API Testing Project for **POSTMAN**</h1>

The scope of this project is to use all  API knowledge gained throught the Software Testing course and apply them in practice, using a live application.

Application under test: **POSTMAN**

Tools used: Postman

Collection link: **https://simple-books-api.glitch.me/books https://reqres.in/api/users https://reqres.in/api/users/2**

<h2>Tests performed</h2>

<ol>
<li>**GET all books**</li>

HTTP method for request: **https://simple-books-api.glitch.me/books**<br>
Request description: **In the first scenario tested, through the GET request, I wanted to bring to view all the existing books, regardless of their nature, the request body returned the total number of existing books**<br>
Test types / techniques used: **The testing techniques used were functional testing, positive testing**<br>
Response status code: **The status code obtained was 200**<br>

Below you can find a picture of the API request from Postman:<br>

<li>**GET all books - filter by negative limit**</li>

HTTP method for request: **https://simple-books-api.glitch.me/books?limit=-5**<br>
Request description: **In the get all books - filter by invalid negative limit scenario, I wanted to bring the number of existing books into view by filtering them using a negative number, the request body returned an error saying that the specified filter number must be greater than 0**<br>
Test types / techniques used: **The testing techniques used were functional testing, negative testing and equivalence partitioning**<br>
Response status code: **The status cde obtained was 400**<br>

Below you can find a picture of the API request from Postman:<br>

**![image](https://github.com/user-attachments/assets/28925c9b-0096-4dbb-92b2-7090a8b6d5d3)**<br>

<li>**Submit order - valid data**</li>

HTTP method for request: **https://reqres.in/api/users**<br>
Request description: **In the submit order - valid data scenario, I wanted to execute a POST request with a bookid and a customername**<br>
Test types / techniques used: **The testing techniques used were functional testing and positive testing**<br>
Response status code: **The status code obtained was 201**<br>

Below you can find a picture of the API request from Postman:<br>

**![image](https://github.com/user-attachments/assets/69582df4-c9fa-421f-8125-21d62a7e0f62) ![image](https://github.com/user-attachments/assets/156ad086-b858-4f80-beef-822baa34b8aa)**<br>

<h2>Execution report for the created API collection </h2>

Below you can find the execution report that was generated through the Postman collection runner. <br>

**![image](https://github.com/user-attachments/assets/3a07a8ba-3155-4d23-b8c7-51d7d6801512)**<br>

<h2>Defects found</h2>

The following issues were identified while running the postman tests:<br>

****An API that creates a GET request, which tries to limit the number of elements revealed, according to a criterion of type number of elements, cannot have negative values, or values over those allowed by the program, so errors will occur when sending the request.**

<h2>Conclusions</h2>

**After testing a set of 10 tests in Postman, covering GET, POST and DELETE requests. Of these, 2 tests generated errors, but these were intentionally designed to cause such results.
Overall, everything went well, with most tests returning expected and positive results. This reflects a robust and stable operation of the system under normal operating conditions.**


