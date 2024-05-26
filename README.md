# Random-User-API-Performance-Test
## Test Scenario
A random API (https://random-data-api.com/api/v2/users) is used for load testing, with the expected load being 120000 in 12 hours. Jmeter has been used to test the performance and stability of the system for 60s, 300s, 600s, and 1200s load.

## Task
- Does Actual TPS(Transaction Per Second) meet the expected required TPS.
- Finding out the Bottleneck/Stress test point of the system.
## Pre-requisite
- Install jdk 11 or any LTS version
- Download and extract Apache Jmeter latest version
- Configure JAVA_HOME and JMETER_HOME in system environment variable
## Task 1. Overall TPS and Load Test Breakdown
## Load Test Strategy
![image](https://github.com/theariful/API-Performance-Test/assets/120745717/701dfd70-1a13-4af4-9281-19785ed6ed24)
## Load Test Results
- Test 1. 60 sec and 166 Users/Threads
![image](https://github.com/theariful/API-Performance-Test/assets/120745717/9259a91d-01e4-4c7c-a070-dcfa0af1419c)
- Test 2. 300 sec and 833 Users/Threads
![image](https://github.com/theariful/API-Performance-Test/assets/120745717/ed6c937f-8699-41c0-b1e3-ac61a9bd2dfd)
- Test 3. 600 sec and 1666 Users/Threads
![image](https://github.com/theariful/API-Performance-Test/assets/120745717/d79d1b23-5d9c-483d-8c1d-6a0b374a5f26)
- Test 4. 1200 sec and 3333 Users/Threads
![image](https://github.com/theariful/API-Performance-Test/assets/120745717/8d8094ac-8950-49c9-9ca9-82255eb5e298)
- Test 5. 1200 sec and 5000 Users/Threads
![image](https://github.com/theariful/API-Performance-Test/assets/120745717/83ccc406-3f34-4048-b910-1b48687a9cd0)
- Test 6. 1200 sec and 6000 Users/Threads
![image](https://github.com/theariful/API-Performance-Test/assets/120745717/66595338-8ba3-494d-926d-3a6b2a5ed938)
- Test 7. 1200 sec and 7000 Users/Threads
![image](https://github.com/theariful/API-Performance-Test/assets/120745717/acfb9f7e-8cd6-4399-943c-e532cb24a061)
- Test 8. 1200 sec and 8000 Users/Threads
![image](https://github.com/theariful/API-Performance-Test/assets/120745717/ff525f1b-ff73-498d-8a74-93ea4efd0a3f)
- Test 9. 1200 sec and 8500 Users/Threads
![image](https://github.com/theariful/API-Performance-Test/assets/120745717/fd3afaea-16e1-4495-9cb1-92f305489035)
## HTML Summary Report
![image](https://github.com/theariful/API-Performance-Test/assets/120745717/be588a32-84ec-4245-aa99-bfcf089202e5)
## Task 2. Finding out the Bottleneck/Stress test point
- Strategy to Finding out the Bottleneck/Stress test point
![image](https://github.com/theariful/API-Performance-Test/assets/120745717/991a710c-bd77-4275-8eaa-7957638796c2)
## The Bottleneck/Stress test point (System starts to show error with 6.5 TPS for 1200 Sec, while handling 8525 user/threads)
![image](https://github.com/theariful/API-Performance-Test/assets/120745717/9bd024bf-c88a-469b-bc6c-7a541c616b25)

