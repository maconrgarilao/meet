# Meet App 
This is an on-going project to build a serverless, progressive web application (PWA) with React using a test-driven development (TDD) technique. The application uses the Google Calendar API to fetch upcoming events.

The project will have the following features with their user stories and scenarios:

<b>Feature 1: Filter events by city</b>

<i>As a user, I should be able to filter cities so that I can see the upcoming events for that particular city</i>

      •	Scenario 1: When a user hasn’t searched for a specific city, show upcoming events from all cities

                    Given a user has just signed up
                    When the user opens the app
                    Then all events will be shown from all events

      •	Scenario 2: User should see a list of suggestions when they search for a city

                    Given a user is looking for a city
                    When the user types letters
                    Then a list of cities should show up 

      •	Scenario 3: When the user searches for city, a list of upcoming events in this city should be shown

                    Given a user has chosen a city
                    When the user clicked the “Search” button
                    Then a list of upcoming events should show up for that particular city

<b>Feature 2: Show/Hide an event detail</b>

<i>As a user, I should be able to have an option to see and hide event detail so that I can have access whenever I want to see events</i>

      •	Scenario 1: An event element is collapsed by default.

                    Given a user chooses a city
                    When the page reloads to the event page
                    Then event details are not shown by default

      •	Scenario 2: User can expand an event to see its detail.

                    Given a user is interested to a particular event
                    When the user clicks the “Details”
                    Then the user should be able to see the list of events

      •	Scenario 3: User can collapse an event to hide its detail.

                    Given an event has been clicked
                    When the user clicks the “Back” button
                    Then the event detail should collapse and go back to original


<b>Feature 3: Specify number of events</b>

<i>As a user, I should be able to modify the number of events I want to see so that I can see more or fewer events in a city at once</i>

      •	Scenario 1: When user hasn’t specified a number, 32 is the default number

                    Given a user has chosen a particular city
                    When the user clicks the page
                    Then 32 upcoming events list is shown

      •	Scenario 2: User can change the number of events they want to see

                    Given a user wants to modify number of events in a single page
                    When the user clicks a specific number
                    Then the page should show the number of events on the particular city

<b>Feature 4: Use the app when offline</b>

<i>As a user, I would like to be able to use the app when offline so that I can see the events I viewed the last time I was online</i>

      •	Scenario 1: Show cached data when there’s no internet connection

                    Given user has previously opened the app with available internet connection
                    When user opens the app without internet connection
                    Then user received cached data from their last session

      •	Scenario 2: Show error when user changes the settings (city, time range)

                    Given user received cached data from last session without internet connection
                    When user changes settings (city, time range)
                    Then user received error message saying data is not available without internet connection

<b>Feature 5: Data Visualization</b>

<i>As a user, I should be able to have an overall view of events so that I can easily pick a city that I want</i>

        •	Scenario 1: Show a chart with the number of upcoming events in each city

                    Given a user opened the app
                    When user scrolls the page
                    Then user should see a quick scan of upcoming events in each city


[User stories and scenarios.pdf](https://github.com/maconrgarilao/meet/files/10860950/User.stories.and.scenarios.pdf)
