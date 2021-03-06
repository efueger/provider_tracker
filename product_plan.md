# Capstone Product Plan

## Product Plan Components
1. __Problem Statement__: Current methods of tracking hours and location of at-home care providers of Department of Rehabilitation    clients do not take into account the lack of reliable technology low-income workers have access to, nor the limited budget of state administrators to support expensive software.  Currently state governments have been purchasing software meant to support hospital field workers, but the software does not adapt well once the software's more expensive features are cut out by the state budgets, and no support is given to clients and workers who attempt to use software meant to be used with landline telephones, fixed verification devices, or later model mobile phones, none of which the state provides.

2. __Market Research__: Outline the key insights from your research, including:
  - COMPETITION 
    - __competing apps__
      - existing system that using landline based calling system (electronic voice verification features are not used) 
      - http://www.sandata.com/our-platform/santrax-electronic-visit-verification
      - http://www.dhs.state.il.us/page.aspx?item=66961
      - GPS tracking apps marketed to companies with field workers
        - http://www.clicksoftware.com/small-medium-business-streetsmart 
    - __non-app solutions__
      - paper timesheet signed by both client and worker.  Still required in Illinois for some reason.  Workers and Clients must submit          these in addition to using automated system. 
    - __research from users on why these alternatives do not effectively address the problem.__
      -  My previous position as a case coordinator at the Illinois Department of Rehabilitation gave me direct user experience with            the Santrax and paper timesheet systems of tracking workers.  In my experience I found the following problems:
        - Both systems required undo time commitment from workers and admins and distracted from client care
          -  paper timesheets required worker to leave client to drop off timesheet at local office twice per month
          -  admins needed to manually check that timesheets matched Santrax, and required that admins contact clients if timesheets                 were illegible or timesheets and santrax logs had mismatched work hours
          -  Santrax system had time-consuming robo-operator that required worker to go through up to ten steps to check in and out and             did not give feedback when worker input incorrect information
          -  bugs in Santrax required admins to repeatedly contact workers and clients to verify hours worked when calls did not log or             were incomplete
    - __differentiation: what makes my idea/product different__
      - by texting in worker ID #'s, workers will be able to see the information they are logging in, and will have better feedback on         typos.  This will cut down on the follow-up and error correcting required from the worker and admin under the previous system.

3. __User Personas__: A summary of your main target user group(s). What are their key characteristics? How do those characteristics factor into project/app/idea?
  - WORKER
  - CLIENT
  - ADMIN(DISTRICT)

4. __Trello Board__:
  - https://trello.com/b/mXAhNW8P/provider-tracker

5. __Technology selections__:
   - Draft Feature Set

      * Database that logs clients, their address, their providers, provider ID #'s, history of provider check ins/outs, and contact         information for clients and providers
      * API that accepts SMS from provider and returns unique link for checking in - then returns time and location information of           check ins/outs to database
      * Administrator interface that displays client and provider information, and alerts administrator of unusual behavior

   - Draft Technology Choices
      * SMS messaging API (Twilio)
      * Live Events (notifications, live updates)
      * Ruby on Rails
      * Heroku
