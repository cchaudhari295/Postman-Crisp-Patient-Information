**Integrated Postman Tests With Github Actions and Generated HTML Report**  


**API endpoint:**
GET https://apimgmt-dev-crisp.azure-api.net/patients/query  

**Query Parameters / Data**

| ID  | Name       | Date       | Location      |
|-----|------------|------------|---------------|
| 111 | Jenn D.    | 1934-06-01 | CA            |
| 222 | Jack       | 1956-05-01 | MD            |
| 333 | Bernard    | 1966-04-01 | CA State      |
| 444 | Ross C.    | 2000-03-01 | Valley State  |  

- Below postman tests are present to test the API endpoint -:  

**1. GetPatientDetailsByIDRequest**

Test 1: Verify the details when valid ID is passed.

Test 2: Verify if the status code is 200

Test 3: Verify if the response time is less than 300ms

**2. GetPatientDetailsByIInvalidDRequest**

Test 1: Verify if the property 'Id' is present in the response

Test 2: Verify the error message when Id is invalid

Test 3: Verify if the status code is 400

**3. GetPatientDetailsByNameRequest**

Test 1: Verify the details when Name is passed

Test 2: Verify if the status code is 200

Test 3: Verify if the response time is less than 300ms

**4. GetPatientDetailsByInvalidNameRequest**

Test 1: Verify if the Name is undefined

Test 2: Verify the error message when Name is invalid

Test 3: Verify if the status code is 400

**5. GetPatientDetailsByAddressRequest**

Test 1: Verify the details when Address is provided

Test 2 : Verify if the status code is 200

Test 3: Verify if the response time is less than 300ms 

**6. GetPatientDetailsByInvalidAddressRequest**

Test 1: Verify when invalid address is provided

Test 2: Verify if the Address is a string

Test 3: Verify the error message when address is invalid

Test 4: Verify if the status code is 400

**7. GetPatientDetailsByValidDateOfBirthRequest**

Test 1: Verify the details when date of birth is passed

Test 2 : Verify if the status code is 200

Test 3: Verify if the response time is less than 300ms 

**8. GetPatientDetailsByInvalidDateOfBirthRequest**

Test 1: Verify when invalid DateOfBirth is passed

Test 2: Verify whether DateOfBirth is a string

Test 3: Verify the error message when DateOfBirth is invalid

Test 4: Verify if the status code is 400    
  

**HTML REPORT**
- To see the report, follow below steps-:
    1. Click on Actions.
    2. Click on the latest workflow run link.
    3. Click on Postman Test Report present in Artifacts section. The report will be downloaded on your system.
    4. Open the HTML report and observe the test results.
