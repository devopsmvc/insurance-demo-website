# Insure-Me (An Insurance Domain Project)

This project will help you to understand various concept related to Insurace domain. Please read the Insurace-domain.pdf to get more functional knowledge on Insurace domain. 

This project uses HTML, CSS and Javascript as frontend and Java Spring Boot for Backend microservice.

Steps to run the project : 
1. Checkout the code.
2. Build the project using 'mvn clean package'.
3. Run the application as Java Application.
4. Access the application at "http://localhost:8080".

<img width="1439" alt="Screenshot 2022-11-03 at 21 10 55" src="https://user-images.githubusercontent.com/114076664/200126590-de9d3dcc-7e21-4e8c-a64a-1dd165dfefcb.png">

The application exposes following APIs : 

1. /hello   -> to test the microservice

2. /createPolicy (method type : POST) -> to create an Insurance Policy
    RequestBody : 
    {
    "policyId": 2,
    "policyHolderName": "Shubham",
    "policyType": "Individual",
    "policyPrice": 10000,
    "policyStartDate": "10-Sep-2021",
    "policyEndDate": "10-Sep-2022"
     }

      //policy id is auto incrementing. so need not to pass while creating.
      
3. /viewPolicy/{policyId} (method type : GET) -> to view the policy details.

4. /updatePolicy (method type: PUT) -> to update the Policy details.
   RequestBody : 
   {
    "policyId": 2,
    "policyHolderName": "Shubham",
    "policyType": "Individual",
    "policyPrice": 10000,
    "policyStartDate": "10-Sep-2021",
    "policyEndDate": "10-Sep-2022"
    }

5. /deletePolicy/{policyId}  (method type: DELETE) -> to delete the Policy details.
