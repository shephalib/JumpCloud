Testing completed for the JumpCloud’s password hashing application in Golang. This application hashes the password provided by the user using SHA512 algorithm and then encodes it using base64 encoding. 
Password hashing application was obtained based on provided instructions and four given endpoints were tested on a windows machine using Git bash CL utility tool for executing curl commands.
--POST call that sends password to the http://127.0.0.1:8088/hash, which in response provides the job identifier and computes the hash.
--GET call  to /hash uses the job identifier generated in the POST call and returns the base64 encoded hash for the password for the job id
--GET to /stats provides the total hash requests sent when server started and average time of the hash request
--POST call  to shut down the application
----------------------------------------------------------------------------------------------------------------------------------------
Test deliverables include:
Test plan provided in the doc format that identifies the objective, scope of the project, features tested/ and not tested along with automation script plan that can be used.
Test cases document is provided in excel sheet with results and screenshots of curl commands along with messages and responses.
-------------------------------------------------------------------------------------------------------------------------------------
Test results:
Out of 25 test cases, 12 Failed. Some of the failed test cases have assumptions as no password rule requirements were provided and no detail on Authentication/Authorization was given as no userid is being used in the POST/GET endpoints.
