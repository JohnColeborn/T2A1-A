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

- Identify a database commonly used in an API project.
    
    While possibly not associated with being commonly used in an API project <b>Google Sheets</b> is an exemplary example of a database commonly used in API projects. Exemplary only in the case of innocence*. Used heavily in low-key, low demand, and low skill API projects.

- Discuss the pros and cons of this database.
    - <b>Pros</b>: 
        - Is widely accessible.
        - Free to use.
        - Easily learnt database. 
        - Its inherent security is excellent (Questionably).
        - It utilises SQL (Limited).
        - Extremely easy to understand overall structure.
        - Accessible from an early understanding point.
        - Shows and allows multiple users at once.

    - <b>Cons</b>
        - Integration with back end is complicated
        - Not scalable due to limited storage
        - Not designed as a database, so functionality overall is lacking
        - Can't store beyond a table
        - Performance drops when used simultaneously.

#  Q3 Discuss an implementation of an Agile project management methodology for an API project.

- What is an Agile methodology? 
    - "Agile methodology is a project management framework that breaks projects down into several dynamic phases, commonly known as sprints". [[1]](#1)

- In the context of implementation, often tools associated with project management are used to map out or "rough" draft an API. They are then used to break down the project into an epic (often centered around specific features), and from the epic broken down further into stories that may be achievable in a single session or days work.

    - Some examples of this include webapps such as Trello, which utilises kanban ideology to achieve this purpose. To further iterate on this example, initially a project will be started in Trello and cards will be created with generic overall information or tasks such as "Create Kanban", "Plot API structure", "Determine features required" etc.

    - These cards are then modified with elements such as comments, priority listings, deadlines, and more. Once the overall Trello path is done it may be broken down further into "smaller chunks" such as on the "Plot API structure" card - adding elements such as "Utilise drawIO to wiremap the API features", "Ensure the relationships are defined e.g.: one to many, many to many or others".

    - Once these initial steps are completed as the first 'sprints', the overall project moves forward similarly to the 'sprints' shift to more advanced elements.


<a id="1">[1]</a>
Laoyan, Sarah (Feb 2 2024)

https://asana.com/resources/agile-methodology

#  Q4 Provide an overview and description of a standard source control process for an API project.

- A common approach to standard source control includes but is not limited to version control software such as Git and focuses around certain aspects to achieve its desired outcome.

    - These aspects include the capacity to backup data, implement multiple simultaneous users, roll back updates, enable tracking on each incoming and outgoing submission.

    - In regard to how this applies to an API project an example would be multiple users working simultaneously on separate functions to be utilised together in the final product. This is achieved through Git by creating and working on separate branches which are upon completion submitted to the main branch to be merged. 

    - After revision and an acceptance by the main branch and supervisor they will be merged and the entire project in the form of the main branch will increase or update to the next version. This entire process is tracked by the source control and enables the supervisor to roll back, reject, accept and use many other beneficial tools.



#  Q5 Provide an overview and description of a standard testing process for an API project.

- An overview of a standard testing process for an API project.
    - Utilising an application such as Insomnia is a commonly sourced solution to testing an API project. Outside particular apps it is effectively integration testing where unit testing is completed based on individual units such as a POST function, and once unit testing is complete it is then tested as an overall with a certain approach. Some approaches include 'Big Bang Approach, and Incremental Approach' [[2]](#2)

    - Some further methods used as a part of testing particularly in Insomnia include the following:

        - After programming a particular feature such as a POST method, Insomnia is used to 'Unit Test' the functions, checking for errors which range from 1xx to 5xx, and providing feedback in order to clarify issues.

        - Another aspect of testing revolves around authentication, where again using Insomnia, a 'Unit Test' can be performed to confirm that correct security protocols and authorisations in general are appropriate. 

<a id="2">[2]</a>
Authors Unknown (Publication Date Unknown)

https://katalon.com/resources-center/blog/integration-testing


#  Q6 Explain the three principles of information system security.

- To identify the 'three' principles.
    - Confidentiality
    - Integrity
    - Availability

- The AU government has an interesting take on these three principles and grow them further into 'five' principles [[3]](#3). These five principles assist in explaining the three.

    - Confidentiality. To govern confidentiality it is necessary to identify assets used, and the associated risks. This then allows implementation of controls to manage the risks. Ensuring that data which is meant to be private remains as such includes methods such as hashing passwords, multifactor authentication, encryption methods such as symmetric or asymmetric encryption and more. 

    - Integrity. Ensures validation of data both sent to and received from a client. This has many forms including controls around specific characters, length of string and size requirements. A common example of integrity principles is limiting the size and format of a file permitted to be sent and received, such as used by Gmail, where files over a certain size or alternate formats are not permitted due to those particular alterations outside the permissible being prone to use as a means of invasion or distortion of integrity.

    - Availability. This sells itself, it is availability through any circumstance. In the case of a power outage, or a DDoS attack, the data behind security remains secure. A somewhat limited example of this is through source control. "*thanks for the memo, had some dodgy power outages this week don't want to lose progress*" (git add . etc)

- To summarise the CIA triad is both astronomically and sadly necessary to ensure that data remains confidential, true to itself, and available when needed.

<a id="3">[3]</a>
https://www.cyber.gov.au/resources-business-and-government/essential-cyber-security/ism/cyber-security-principles

#  Q7 Provide an overview of what would need to be done within an API project to implement at least one of the principles explained in Question 6. 

- Confidentiality. In the example of an API, there are many factors of authentication and verification available as a means to ensure data verity and security. These include, but are not limited to, the use of tokens, passwords, possessions (phones, pcs), physical attributes (fingerprints, retinas). 

    - As an example based around a data breach, copying somebody's fingerprint to access their phone. This involves biometric security or 'physical attributes' and may be accessed via "using a picture of the target's fingerprint" [[4]](#4).

    - To parallelogram a little here a *browser fingerprint* collects data about a client in the same way that a biometrical fingerprint does. As a unique identifier of the client it is frequently used as a means of identification and verification. 

    - As with a physical fingerprint, a browser fingerprint also is able to be tracked, 'stolen', and used adverse to confidentiality. Some means to prevent this include using a VPN, proxies, and masking.

    - Within an API project, to implement confidentiality an example would be using hashed passwords, token authorisations, two-factor auth, and more. The concept is focusing on obfuscation and limitation.

    - Obfuscation. Deliberately rerouting a source of data. EG: Torrents somewhat infamously known due to sites such as ThePirateBay. Hashing passwords, ensuring that data available to a client is unable to be accessed outside of the user to retrieve sensitive data. Seen also in .env being hidden in our particular project. 

    - Limitation. Deliberately limited file handling. EG: Password must contain one capital, one special character, and be more than 9 digits. Hard coded varchar with a limitation of twenty elements may enforce a degree of security against brute forced or spammed infiltration.  

<a id = "4">[4]</a>
Mott, Nathaniel (Nov 23 2021)

https://au.pcmag.com/security/91051/hacking-fingerprints-is-actually-pretty-easy-and-cheap

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

