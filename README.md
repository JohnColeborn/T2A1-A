#  Q1 Describe the architecture of a typical API project, such as a Flask application.

## Definition of an API
- An application programming interface

    The architecture of an API is summarised as a series of steps through programming syntax wherein interaction from a client is sent to a server and given a response. 

    The client may include system queries, web queries, personal queries or more. 

    The architecture of a typical API project includes but is not limited to the following, focusing around 7 points:

    <b>1 - POST</b>. A login form or 'POST' submission handling, where input is taken from the front end, processed through appropriate channels, often including verifications and security, and returned as a true or false authorisation.

        - An example of this is a classic login, where if the stored information is correct the login will be granted and it continues to the next step (2. - GET), else if it is incorrect it will return an error (hopefully well handed) that informs the client of incorrect submission.

    <b>2 - GET</b>. Submission handling of a return of information from the server such as in a 'GET' request. Where after being authorised and verified the API accesses the database and returns to the client information typically set aside for the specific client.

        - EG: Logging into a social media platform such as Facebook returns to the client personalised data retrieved from the database. "Your Feed"

    <b>3 - PUT</b>. PUT is used to entirely replace all associated fields. An extremely important thing to note is that it requires <b>all</b> fields relevant to be modified. 

        - EG: Having not accessed a particular server for 10 years, 'webapp' has verified and authorised the client to update details based on successful POST. Fields include name, email, password, contact number, address. 

    <b>4 - PATCH</b>. PATCH is extremely similar to PUT in terms of handling, where the input is treated as an alteration of existing data. The main difference between the two is PATCH is only required to replace partial data from an array of fields, whereas PUT is required to replace all data from the same. 
        
        - EG: Having not accessed a particular server for 10 years, 'webapp' has verified and authorised the client to update details based on successful POST. Choose from one or all fields including name, email, password, contact number, address. 

    <b>5 - DELETE</b>. DELETE sells itself as far as a concept goes. 
    Only possible upon existing data, else incurring an error. Ideally only an authorised, verified client is capable of this submission.

        - EG: Posted something on facebook that wasn't liked in retrospect, and hence deleted.

    <b>6 - OPTIONS</b>. An OPTIONS call is similar to looking at a menu at a restaurant. The client sends OPTIONS request to the server effectively asking what is available. 
     
        - EG: At a restaurant with no menus available we query the server (unintentional double entendre) on what is available. The server responds with relevant information.

    <b>7 - HEAD</b>. HEAD is in a nutshell, in a nutshell. Mainly comprised of metadata handling, it requests a synopsis of the data encased in the body/database.

        - EG: To get a summary of what a book is about is generally contained in the prefix





#  Q2 Identify a database commonly used in an API project (such as a Flask application) and discuss the pros and cons of this database.



#  Q3 Discuss an implementation of an Agile project management methodology for an API project.

#  Q4 Provide an overview and description of a standard source control process for an API project.

#  Q5 Provide an overview and description of a standard testing process for an API project.

#  Q6 Explain the three principles of information system security.

#  Q7 Provide an overview of what would need to be done within an API project to implement at least one of the principles explained in Question 6.

#  Q8 Explain the legal obligations that developers of a social media website or social media application would have in regards to handling user data, with reference to any applicable laws or acts.

# Q9 Describe the structural aspects of the relational database model. Your description should include information about the structure in which data is stored and how relations are represented in that structure.

#  Q10 Describe the integrity aspects of the relational database model. Your description should include information about the types of data integrity and how they can be enforced in a relational database.

# Q11 Describe the manipulative aspects of the relational database model. Your description should include information about the ways in which data is manipulated (added, removed, changed, and retrieved) in a relational database.

# Q12 Conduct research into a web application (app) and answer each of the following sub-questions:

   - List and describe the software (tech stack) used by the app. 
   - Describe or make educated guesses about the hardware used to host the app.
   - Describe the interaction of technologies within the app.
   - Describe the way data is structured within the app’s database(s).
   - Identify the entities/tables that are tracked within the app’s database(s).
   - Identify the relationships and associations between the entities/tables identified in sub-question E.
   - Design an entity relationship diagram (ERD) based on the answers provided to sub-questions E and F. This must represent a relational database model, even if the app itself uses something other than a relational database model.

