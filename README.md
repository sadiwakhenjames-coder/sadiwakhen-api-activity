1. Markdown
2. # RESTful API Activity - [Khen James Sadiwa]
3. ## Best Practices Implementation
4. **1. Environment Variables:**
5. - Why did we put `BASE_URI` in `.env` instead of hardcoding it?
6. - Answer: We used `BASE_URI` to use the actual base uri in the .env because using `.env` separates it from the code that
            is sent to the Git Repository. It is said that `PORT`s and ``BASE_URI`s are very sensitive data and should not be
            just sent like that, so we use  `.env` as as safety measure.
7. **2. Resource Modeling:**
8. - Why did we use plural nouns (e.g., `/dishes`) for our routes?
9. - Answer:    Grammatically speaking, using plural just really makes sense since there are multiple records in the
                list(`rooms`) another reason is because `rooms` is the name of the list where the data resides which made 
                visible by the `module.export: rooms;`.
10. **3. Status Codes:**
11. - When do we use `201 Created` vs `200 OK`?
        We usee `201 created` when the http method is POST because the POST method creates a new record in the database whereas `200 OK` is used when we are indicating a successful GET method.
12. - Why is it important to return `404` instead of just an empty array or a generic error?
13. - Answer:   I actually experienced from a website where it said that the website encountered an error, now they don't 
                explicitly said what triggered the error. I am annoyed because do i really need to get through who knows how much
                troubleshooting before resolving the problem. In using error codes, debugging will be easier because you'll know what triggered the error and where the error is.
14.
15. **4. Testing:**
16. Attached among the files in the folder `sadiwakhen-api-activity`, named `Test.png`
