# bsd-find-movie-app (Find Movie App)

## Requirement

* Get free API key from OMDb API, (or any similar movies API you can find). Study the documentation before starting implementation.
* The website looks similar to the design (Desktop and Mobile) and is available for users through a link.
* On the initial page load, the "YOU MIGHT LIKE" section should be filled with either random movies or predefined ones. (prepare a list of movies upfront and trigger API request to fetch them before rendering the page)
* Users can find movies using the search bar, request to the API should trigger after entering a minimum of 2 characters and be debounced to prevent too many requests at once. (no enter click, listen to keypress and fetch data after e.g. 300 milliseconds delay, try to avoid fetch on the first character typed in)
* When users use the search bar, the "YOU MIGHT LIKE" section should be replaced by search results (movies that were found in the API), if the search bar is cleared, bring back the "YOU MIGHT LIKE" section again.
* When users click on the movie, a full-page dialog window should show up, hiding the current page content and presenting a particular movie (get details from the API) in a card component. Users should be able to close the dialog by clicking the "X" icon and/or on the background around the card.
* Handle loading and errors in the code appropriately. (handle error first, then loading, then data)