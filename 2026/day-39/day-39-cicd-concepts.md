## Task-1 : The Problem " Think about a team of 5 developers all pushing code to the same repo manually deploying to production."
  - Solution: "What can go wrong?" -- When the team of 5 developers pushing code to the same repository , problem may occurs like:
    - Code conflict : When two developers changes the same file and push the code , merge conflict can happens that can break the application.
    - Broken Production : If a developer can push the code to the production without checking the error the application can be crashed in the production.
    - Human error : Mannual deployment may cause some errors (like missing files, wrong commands etc ) that can break the whole system.
  - "it works on my machine" : It means the code runs correctly and smoothly in the developer's local system but failed to run on another developer's system or on production. This my happen because of different environment :
    - different os
    - different environment variables
    - different (missing) dependencies
    - different library versions
  - "How many times a day can a team safely deploy manually?" : mannual deployment may takes a lot of time , so that they can deploy very few times in a day usually 1 or 2.
- Task-2 :  CI vs CD
  -  
  
