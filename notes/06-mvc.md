# MVC

MVC - Application design pattern, that is the most tried and true method of designing an application.
    MODEL - VIEW - CONTROLLER

    VIEW - what the user sees and interacts with
    CONTROLLER - takes in actions from users and interprets them
    SERVICE - adds rules to what the controller takes in
    APPDATA - stores all the information
    MODEL - blueprints for data that is communicated back to the controller


        - OBSERVER PATTERN: a design pattern that can be used as a part of MVC to help pull it off, and help make the appstate actually work
    
    CONSTRUCTOR = KEY WORD a special function used for building/instantiating a class or an instance of a class
            THIS MEANS TO GIVE ME AN INSTANCE OF SOMETHING - USING THE MODEL + DATA/rawMaterial

            PASS AN OBJECT INTO A CONSTRUCTOR in order to fill out the data needed
            generateId() => use for week3, we won't use this after // DATABASE WILL GENERATE AN ID AFTER WEEK 3

            when we use the "new" keyword, we create a new instance of the controller

    IF INFORMATION OR CODE IS NOT INSIDE OF A "export" class IS PRIVATE or LOCALLY SCOPED
    IT IS NEVER THE JOB OF THE CONTROLLER TO MODIFY DATA
    
    SINGLETON PATTERN: service layer exports singletons. THERE IS ONLY ONE SERVICE