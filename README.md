# bsd-find-movie-app (Find Movie App)

## Requirement

* Get free API key from OMDb API, (or any similar movies API you can find). Study the documentation before starting implementation.
* The website looks similar to the design (Desktop and Mobile) and is available for users through a link.
* On the initial page load, the "YOU MIGHT LIKE" section should be filled with either random movies or predefined ones. (prepare a list of movies upfront and trigger API request to fetch them before rendering the page)
* Users can find movies using the search bar, request to the API should trigger after entering a minimum of 2 characters and be debounced to prevent too many requests at once. (no enter click, listen to keypress and fetch data after e.g. 300 milliseconds delay, try to avoid fetch on the first character typed in)
* When users use the search bar, the "YOU MIGHT LIKE" section should be replaced by search results (movies that were found in the API), if the search bar is cleared, bring back the "YOU MIGHT LIKE" section again.
* When users click on the movie, a full-page dialog window should show up, hiding the current page content and presenting a particular movie (get details from the API) in a card component. Users should be able to close the dialog by clicking the "X" icon and/or on the background around the card.
* Handle loading and errors in the code appropriately. (handle error first, then loading, then data)

## Additional Requirements

* To avoid working on a real API and burning its daily limits, implement a mock server first (try to recreate original schema/data format), code the app, and when it'll be ready switch to the real movies API (e.g. OMDb) for final testing if all works nicely together.
* Improve loading and error handling by using e.g. additional components, texts, assets as presented on the last views of the design.
* Implement more fields from the API, explore, discover what's available and make it as robust as it's possible. Use all the data! 🔥
* Don't show too many movies at once, limit to e.g. 10 of them, use lazy loading for fetching more.
* Add API tests to your code, using e.g. jest.
* Add e2e tests to your code, using e.g. cypress.