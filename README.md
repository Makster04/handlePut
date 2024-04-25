# HandlePUT

## Route: 
/customers/{id}

## Input: 
JSON body containing the updated data and ID (##) of the record to be updated.

## Output: 
Object representing the updated record.

## Function Mapping:
Lambda Function: 
[handlePut](https://us-west-1.console.aws.amazon.com/lambda/home?region=us-west-1#/functions/handlePut?tab=code)

## Data Flow:
1. Client sends a PUT request with JSON body to {root_url}/people/{id}.
2. Amazon API Gateway triggers the handlePut Lambda function.
3. Lambda function updates the record with the specified ID in the database.
4. Lambda function returns the updated record as the response.
5. Amazon API Gateway sends the response back to the client.
