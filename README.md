# Frontend Design Document

## Abstract
With increasing pressure from climate change, deforestation, pollution, and other threats that require urgent attention and collaborative action the evergreen initiative was born.
The Evergreen Initiative is a web application designed to provide users/farmers with valuable information about soil types, climate conditions, and suitable plants for cultivation based on their location as well as machinery to aid the process.
Knowing what crops would thrive in favourable growing conditions and availability of the farm machinery will potentially increase agricultural crop production significantly.

## Component tree diagram of the feature
![Model](https://raw.githubusercontent.com/DeraJSP/evergreen-initiative/main/components-tree.png)

## Flow diagram API execution
![Model](https://raw.githubusercontent.com/DeraJSP/evergreen-initiative/main/api-flow.png)
Access to the Evergreen API does not require authentication for public endpoints. However, certain endpoints may necessitate authentication for specific operations such as creating or updating user data.

The Evergreen API integrates with external APIs to provide additional functionalities:

OpenWeatherMap API: Used to retrieve climate information based on latitude and longitude coordinates.

Endpoint: https://api.openweathermap.org/data/2.5/weather?lat={latitude}&lon={longitude}&appid={API key}
Google Maps API: Utilized to fetch map images of specified locations.

Endpoint: Google Maps Static API
ISRIC SoilGrids API: Accessible to retrieve soil information based on geographic coordinates.

Endpoint: https://rest.isric.org/soilgrids/v2.0/
FAO BigQuery API: Provides crop data and information for agricultural analysis and research.

## Error handling
Automated Testing using Test cases that cover potential error scenarios will help identify issues early in the development cycle. We will be creating these test cases using Jest v29.7.

## Alternative design considerations
- Different layout options for the user interface
- Multiple colour schemes and typography choices
- Alternative navigation structures (e.g., tabs vs. dropdown menus)
- Different approaches to handling user input validation
- Responsive design for different screen sizes

## Technologies and tools used 
- React
- Css
- Vscode
- Clickup
- Github
- NPM

## Test scenarios 
- Testing the user interface across different browsers (Chrome, Firefox, Safari, etc.)
- Verifying respionsiveness on different screen sizes
- Evaluating load times and performance under different network conditions
- Testing user acceptability with a prospective user

 ## Accurate estimate of work and level of parallelization
- Tasks should be divided into smaller subtasks, with completion times estimated for each.
- Finding dependencies between activities to identify potential for parallelization
- Team size and availability of team members will be considered when estimating work
- Use of Kanban boards to visualize the timeline and parallelization of tasks

  ## Click interaction structure
![Model](https://raw.githubusercontent.com/DeraJSP/evergreen-initiative/main/click-interaction-structure.png)
