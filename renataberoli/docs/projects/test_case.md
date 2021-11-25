# Testing GitHub Search API with python unittest
- **Project Name:** Testing GitHub Search API with python unittest 
- **Module Name:** Searching for repositories 
- **Reference Document:** [Github Docs](https://docs.github.com/en/search-github/searching-on-github/searching-for-repositories) 
- **Test Scenarios:** Positive Testing + Optional Parameters 
- **Created By:** Renata Beroli 
- **Date of Creation:** 24/11/2021

| Test Action Category | Test Action Description |
| --- | --- |
| `Validate status code:` | 200 OK for GET requests  |
| `Validate payload:` | Response is a well-formed **JSON object**. |
| `Validate state: ` | N/A |
| `Performance sanity:` | N/A |

---

## Test Cases

Those Test Cases bellow were executed and automatized in my GitHub --> [Unittest - GitHub API](https://github.com/renataberoli/Unittest_Python)

### ReposNameTC
| Description | Test Data | Expected Result | 
| ----------- | --------- | --------------- | 
| This test aims to confirm that the GitHub Search API returns just the result that matches the repository's name searched. | The keyword "Python" is in the name. | The GitHub API returns a list of repositories with the specific name that was searched. |
**Comments:** N/A

----

### ReposDescriptionTC
| Description | Test Data | Expected Result | 
| ----------- | --------- | --------------- | 
| This test aims to confirm that Github Search API returns the repositories that have in the description the keyword searched. | The keyword "Python" is in the description. | The GitHub API returns one or more repositories that have the word “Python” in your description. | 
**Comments:** N/A

----

### ReposReadmeTC
| Description | Test Data | Expected Result | 
| ----------- | --------- | --------------- | 
| This test aims to confirm that GitHub Search API returns the repositories that have in the readme the keyword searched. | The keyword “Cadmio” is in the readme. | The GitHub API returns one or more repositories with the word “Cadmio” in your readme. |
**Comments:** N/A

----

### ReposOwnerTC
| Description | Test Data | Expected Result | 
| ----------- | --------- | --------------- | 
| This test aims to confirm that GitHub Search API returns just the repository of the specific patch. | The repository path “renataberoli/renataberoli.github.io”. | The GitHub API returns only the specific repository searched. |
**Comments:** N/A

----

### ReposUserTC
| Description | Test Data | Expected Result | 
| ----------- | --------- | --------------- | 
| The test aims to confirm that GitHub Search API returns only the repositories of a specific user. | The user “renataberoli” is the user. | The GitHub API returns only the repositories of “renataberoli”. |
**Comments:** N/A

