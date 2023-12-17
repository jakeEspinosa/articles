Users want a fast and responsive experience and may leave if the webpage is slow. There are many ways to improve the user experience, but an easy win is to filter data on the business logic layer or data layer rather than the front end.

## Why?
Typically, we want the front end to do the least amount of work necessary. Each action the front end takes adds latency and detracts from the user experience. Some things like API calls are unavoidable, but the API should return data in a ready-to-display format so the front end only has to display the information. The front end should not filter the data when the business logic layer or data layer can. Ideally, the data layer should have a SQL view or function that the business logic layer can query. The business logic layer can also filter the data, but this is less performant than having the database do the filtering. 

### Separation of Concerns
A big part of good software development is the separation of concerns or partitioning an application into sections with logical responsibilities. This type of architecture is called an "N-tier" architecture, with N representing the application's number of layers. A typical 3-tier application is split into the front end, business logic, and data layers.

The front end should be responsible for fetching and displaying data. The business logic layer should be responsible for data processing, such as creating accounts, confirming purchases, etc. The data layer should be responsible for storing and filtering data. Each layer should be independent of the others' responsibilities, but the realities of development usually prevent this ideal from being achieved.

## Takeaway
Enforce separation of concerns to improve your front end performance. Have the data layer or business logic layer handle data processing (including filtering) and let the front end handle displaying data. This will improve front end performance and make users happier.
