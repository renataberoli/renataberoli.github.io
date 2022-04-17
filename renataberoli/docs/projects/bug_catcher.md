## Getting started
![Gif home](https://github.com/renataberoli/bug_catcher/blob/main/app/static/img/gif%20principal.gif?raw=true)

### Try a live Demo

###### url
```sh
https://renataberoli.pythonanywhere.com/
```
###### user
```sh
renataberoli
```
###### password
```sh
123and4
```
<br>

### About the project
Bug catcher is a pet-project loosely inspired by GitHub Issues and designed with the primary goal of improving my 
skills in the Django framework.

#### Sketch

The sketch is the most basic structure I designed within the project. It's an excellent way to put the ideas on paper 
and start initial tests. Also, working as a developer, I use the sketch to understand the structures of information and 
draft the models I need to create my system.

![Sketch](https://github.com/renataberoli/bug_catcher/blob/main/app/static/img/sketchs.png?raw=true)

#### The solution
After sketching the interfaces and the system architecture, I translate my sketch into a coding interface with Bootstrap.

![Desktop](https://github.com/renataberoli/bug_catcher/blob/main/app/static/img/bug%20catcher%20desktop%20mock.png?raw=true)

#### Responsive layout
I focused the development on working primarily in desktop systems but was careful to keep minimum responsiveness in 
mobile devices.

![Mobile](https://github.com/renataberoli/bug_catcher/blob/main/app/static/img/mobile%20mock%20bc.png?raw=true)

#### Tech stack
![Django Version](https://img.shields.io/badge/Django-~4.0.3-blueviolet)
![Bootstrap Version](https://img.shields.io/badge/Bootstrap-5-blue)
![HTML](https://img.shields.io/badge/HTML-5-red)
![CSS](https://img.shields.io/badge/CSS-3-yellow)

## Test cases
??? example "Test Cases Plan"

    ### Scenario 1 - Login
    ###### test_login_failed
    | Description | Test Data | Expected Result | 
    | ----------- | --------- | --------------- | 
    |The test aims to check if the user can access the system if the login fails. |Use: username - “beroli”; password - “1234”|The system will return an error asking the user to enter a correct username.|
    
    ###### test_login_success
    | Description | Test Data | Expected Result | 
    | ----------- | --------- | --------------- | 
    |The test aims to check if the user will be redirected to the main page if the login is successful.|Use:  username - “renataberoli”; password - “123and4”|The user will be redirected to the “list of issues” page.|
    
    ### Scenario 2 - List filters
    ###### test_search_filter
    | Description | Test Data | Expected Result | 
    | ----------- | --------- | --------------- | 
    |This test aims to check if the search field works as expected.|Use: Use: “error” as the search argument.|The system will return only issues with “error” in some parts of the title.|
    
    ###### test_priority_filter
    | Description | Test Data | Expected Result | 
    | ----------- | --------- | --------------- | 
    |The test aims to check if the priority field works as expected.|Use: Use: “urgent” as the field’s option.|The system will only return issues with “Urgent” priority.|
    
    ###### test_status_filter
    | Description | Test Data | Expected Result | 
    | ----------- | --------- | --------------- | 
    |The test aims to check if the status field works as expected.|Use: Use: “closed” as the field’s option.|The system will only return issues with the status “closed”.|
    
    ###### test_all_filters_together
    | Description | Test Data | Expected Result | 
    | ----------- | --------- | --------------- | 
    |The test aims to check if all the list filters work together as expected.|Use: search argument - “error”; priority - “urgent”; status - “open”; label - “frontend”; assigned - “renataberoli”.|The system will only show the issue that matches all the filter's arguments.|
    
    ### Scenario 3 - Create issue
    ###### test_issue_creation
    | Description | Test Data | Expected Result | 
    | ----------- | --------- | --------------- | 
    |The test aims to check if the issue's creation is working as expected.|Use: title - “Test issue if issue is created”; project - “Acme”; status - “open”; assignee - “renataberoli”.|The system will create a new issue and redirect the user to the detail view.|

<br>

## Conclusion
In this project, I learned:
- Django framework
- Bootstrap 5.0
- Testing in Django framework
- How to create good documentation for the project
