![image](https://github.com/user-attachments/assets/6d6c79db-407d-48bf-b22c-f2f08c6042b3)<h1>API Testing Project for **POSTMAN**</h1>

The scope of this project is to use all  API knowledge gained throught the Software Testing course and apply them in practice, using a live application.

Application under test: **POSTMAN**

Tools used: Postman

Collection link: **https://simple-books-api.glitch.me/books https://reqres.in/api/users https://reqres.in/api/users/2**

<h2>Tests performed</h2>

<ol>
<li>**GET all books**</li>

HTTP method for request: **https://simple-books-api.glitch.me/books**<br>
Request description: **In primul scenariu testat, prin prisma requestului de tip GET, am dorit sa aduc la vedere totalitatea cartilor existente, indiferent de natura acestora, body-ul requestului a returnat numarul total de carti existente**<br>
Test types / techniques used: **Tehnicile de testare folosite au fost testare functionala, testare pozitiva**<br>
Response status code: **Status code-ul obtinut a fost 200**<br>

Below you can find a picture of the API request from Postman:<br>

**Inserati aici o poza cu requestul din postman in care sa se observe request method, endpoint, request body si response body**<br>

JavaScript Tests:

**![image](https://github.com/user-attachments/assets/e4ebb921-31d5-4afb-a010-250134ad4bf9) ![image](https://github.com/user-attachments/assets/1d36a5ef-3a88-47cf-a775-836f2fa76d0a)**<br>


<li>**Nume Request 2**</li>

HTTP method for request: **https://simple-books-api.glitch.me/books?limit=-5**<br>
Request description: **In scenariul get all books - filter by invalid negative limit, am dorit sa aduc la vedere numarul cartilor existente prin filtrarea acestora, utilizand un numar negativ, body-ul requestului a returnat o eroare care spune ca numarul specificat al filtrarii trebuie sa fie mai mare decat 0**<br>
Test types / techniques used: **Tehnicile de testare utilizate au fost testarea functionala, testarea negativa si equivalence partitioning**<br>
Response status code: **status code-ul returnat a fost 400 Bad Request**<br>

Below you can find a picture of the API request from Postman:<br>

**![image](https://github.com/user-attachments/assets/28925c9b-0096-4dbb-92b2-7090a8b6d5d3)**<br>

JavaScript Tests:

****<br>

.............

<li>**Submit order - valid data**</li>

HTTP method for request: **https://reqres.in/api/users**<br>
Request description: **In scenariul de tip submit order - valid data, am dorit sa execut un request de tip POST care sa aiba un bookid si un customername**<br>
Test types / techniques used: **Tehnicile de testare folosite au fost testare functionala si testare pozitiva**<br>
Response status code: **Status code-ul obtionut in urma requestului a fost 201**<br>

Below you can find a picture of the API request from Postman:<br>

**![image](https://github.com/user-attachments/assets/69582df4-c9fa-421f-8125-21d62a7e0f62) ![image](https://github.com/user-attachments/assets/156ad086-b858-4f80-beef-822baa34b8aa)**<br>

JavaScript Tests:

**Inserati aici o poza cu testele in java script pe care le-ati definit impreuna cu rezultatele executiei acestora**<br>

</ol>

<h2>Execution report for the created API collection </h2>

Below you can find the execution report that was generated through the Postman collection runner. <br>

**![image](https://github.com/user-attachments/assets/3a07a8ba-3155-4d23-b8c7-51d7d6801512)**<br>

The collection was also run through newman directly from the terminal, and the results can be found below:<br>

**Inserati aici o poza cu raportul de executie din Newman**<br>

<h2>Defects found</h2>

The following issues were identified while running the postman tests:<br>

****Un API care creează un request de tip GET, care incearca sa limiteze numarul de elemente dezvaluite, in functie de un criteriu de tip numar de elemente, nu poate avea valori negative, sau valori peste cele admise de catre program, astfel vor aparea erori la trimiterea requestului.**

<h2>Conclusions</h2>

**In urma testarii unui set de 10 teste în Postman, acoperind requesturi de tip GET, POST și DELETE. Dintre acestea, 2 teste au generat erori, însă acestea au fost intenționat concepute pentru a provoca astfel de rezultate.
Per ansamblu, totul a decurs bine, cu majoritatea testelor returnând rezultatele așteptate și pozitive. Aceasta reflectă o funcționare robustă și stabilă a sistemului în condiții normale de operare.**


