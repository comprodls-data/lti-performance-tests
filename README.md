# LTIGW Performance Test

The test will confirm the performance of LTIGW APIs under Load conditions.

### Scope

### Modules Covered
- LTI Gateway
	- API Gateway
	- 6 Lambda Functions
	- SNS topic
- Scoring Layer
	- SQS
	- 1 Lambda Function
### Modules not covered
- Metrica (Test tool would be stubbed in place of Metrica) 
- Konakart (Not part of LTI performance test)
- C1 (Will be covered as part of C1 performance test)

### Objectives of the test
- Identify API response time threshold value
- Behaviour of system under Load

### Test Details
- Total Real Concurrent Users - ?
- Test Duration - 55 min
- Transaction Throughput - ?

## Test data

### For Users:
- A user with role student and is provisioned to shared org.
- All C1 students are provisioned to shared org.
- This test data can be extracted from existing C1 performance test data.

### For Scores:
- Sample json file for partial and complete scores feedback.

### Test scenarios defined 

- Student launches an IELTS test (3 APIs - Invoke, OIDC (GET) & Keyset)
- Student launches and submits an IELTS test (6 APIs - Invoke, OIDC (GET), Keyset, Oauth, Scores, Return)

### What will you monitor? 
- API Response time
- API Errors
- Performance Indexes for Lambda, SNS, SQS and API GW
- Kibana

## Test Report
- Result Summary
- Performance Metrices of Components
- Any Issues
