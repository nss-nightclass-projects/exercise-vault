# The Travel Blog

You've been asked to put together a simple application for your client, Mira. Mira is a travel blogger who creates both videos and writes blog posts for her website. She tries to travel to three destinations per month, spending a week in each place. Then she takes a week off before starting the whole cycle again. She has requested a application where she can add points of interests for the next set of three places she will be visiting. She would like to be able to add points of interest to her destinations so she can have a list of places she needs to visit when she travels. As she visits each point of interest, she would like to be able to edit the point of interest by adjusting the cost and adding a review. She has also asked to be able to delete points of interest from her list. But to ensure she does not accidentally delete anything, she would like an alert to to confirm the delete action.

Mira expects an application that has a clean user interface with easy to read text and an intuitive interface.

To start you off, here's what the resources in your API should look like for this application:

### Places

```json
{
  "locations": {
    "location1": {
      "id": 1,
      "name": "Rome",
      "country": "Italy",
      "dates": "1/1/2021 - 1/7/2021",
      "isCompleted": false
    },
    "location2": {
      "name": "Paris",
      "country": "France",
      "dates": "1/8/2021 - 1/14/2021",
      "isCompleted": false
    },
    "location3": {
      "name": "Everglades National Park",
      "country": "United States",
      "dates": "1/15/2021 - 1/21/2021",
      "isCompleted": false
    },
    "location4": {
      "name": "Zion National Park",
      "country": "United States",
      "dates": "12/8/2019 - 12/14/2029",
      "isCompleted": true
    },
    "location5": {
      "name": "Kyoto",
      "country": "Japan",
      "dates": "12/15/2019 - 12/21/2029",
      "isCompleted": true
    }
  }
}
```

### Interests

An example of what an interest would like when it is initially added:
```json
{
  "interests": {
    "interest1": {
      "locationId": "location2",
      "name": "Eiffel Tower",
      "description": "An object of discord, desire and fascination, the Eiffel Tower never fails to impress. Enriched by a history full of new developments, here you can discover all of its key information.",
      "cost": 16.60,
      "review": "View from the top is amazing"
    }
  }
}
```

## Acceptance Criteria
Below is a starting point for all the technical requirements.  Each acceptance criteria section should be its own ticket.  You should write the appropriate user story to go with each ticket.  Requirements are intentionally left a little vague so you have the freedom to make it your own.


**Given** a user has already has locations <br />
**When** the user opens the application <br />
**Then** all locations should clearly be shown  <br />
**And** it  should be clear which locations have been visited and which have not

**Given** a user wants to keep track of a new location <br />
**When** the user opens the application <br />
**Then** a form should be presented to the user in which they can enter in the location information.

**Given** a user has already has points of interests <br />
**When** the user opens the application to a specific location <br />
**Then** all points of interests should be displayed with their name, description, cost, review if it's not blank and the place it is located

**Given** a user wants to keep track of a new point of interest <br />
**When** the user opens the application <br />
**Then** a form should be presented to the user

**Given** a user has entered in all details of a point of interest <br />
**When** the user performs a gesture to save the point of interest <br />
**Then** the point of interest should be displayed in the application

**Given** a user wants to change the cost of a point of interest or add/change the review to a point of interest <br />
**When** the user performs a gesture to edit the point of interest <br />
**Then** the user should be presented with a form that has the cost and review, if it's not blank, pre-filled <br />
**And** there should be an affordance to save the edited cost and review

**Given** a user has saved a point of interest <br />
**When** the user visits their application <br />
**Then** all points of interest should be displayed <br />
**And** each point of interest should have an affordance to delete it

**Given** a user wants to remove a previously stored point of interest <br />
**When** the user performs a gesture on the delete affordance <br />
**Then** the user should be prompted to confirm the delete

**Given** a user is viewing the delete prompt <br />
**When** the user selects the confirmation affordance <br />
**Then** the point of interest should be deleted <br />
**And** the confirmation message should disappear <br />
**And** the list of points of interest should be refreshed

**Given** a user is viewing the delete prompt <br />
**When** the user selects the cancel affordance <br />
**Then** the point of interest should NOT be deleted <br />
**And** the confirmation message should disappear

## Technical Requirements

1. The application should be built in a modular way in accordance with the principle of _Separation of Concerns_.
1. For persistent data storage, use firebase
1. Routing - you can use it or not totally your decision
1. Bootstrap - at minimum use the grid
1. No linting errors