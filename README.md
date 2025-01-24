# Star Wars API Project

## Overview
The Star Wars API Project is a web application that enables users to explore data from the Star Wars universe by interacting with the Star Wars API (SWAPI). The project focuses on gathering information about the user's character preference, allowing users to compare the selected character data against the rest of the Star Wars world, and visualize it through graphs. This project aims to provide insights into various attributes of Star Wars entities.

## Features and Usage
- Retrieve and display information on various Star Wars characters, species, homeworlds and yes, even spaceships from the SWAPI.
- Collect user preferences to create a new DataFrame for analysis:
- The user will start their journey in this world by being asked:"What character would you like to be today?"
- They will then be presented with a list of character genders to select from
- After that selection, they will be asked what hair color will want (from a list of remaining options)
- And finally, they will be asked what eye color they want (from a list of remaining options)

The result will then use the selected character for comaprison analysis to the rest of the Star Wars ecosystem.
- Generate visualizations (e.g., bar charts, scatter plots) to analyze relationships between different attributes examples: 
* Home world - orbital rotation, population, surface water 
* Species - Height, Average life span, eye colors, skin colors
* Characters - height, weight
* Starships - speed, size ,ship speeds, character heights.

- Easy-to-use interface for searching and selecting specific characters and learning how their information compares to the rest of the Star Wars ecosystem.

## Technologies Used
- Fetch API for interacting with SWAPI root:
https://www.swapi.tech/api/
- Data manipulation with Python 
- Pandas, Json, Numpy, Urllib.request, Matplotlib.pyplot

## Data Collection
Users can collect data by selecting the following:
- Characters: Users can select character details such as gender, hair color, and eye color.
The selected data is used to create a new DataFrame for further analysis and visualization.

### Example Data Collection Process:
1. A user selects a character through a question and answer process.
2. The application retrieves and stores the selected data into a structured format (e.g., an array of objects).
3. This data is transformed into a DataFrame, where each entry corresponds to a spaceship and the associated character(s).

## Data Analysis and Visualization
After data collection, the project analyzes relationships between different attributes of the selected characters. Users can visualize:
- **Character Heights**: A scatter plot to explore any correlation between these two metrics.
- **Crew Size of Spaceships**: A bar chart showing the number of crew members per spaceship.

### Visualization Examples:
1. **Scatter Plot of Spaceship Speeds vs Character Heights**
- This graph illustrates whether there's a significant correlation between the speed of the ships and the heights of characters.
2. **Bar Chart of Spaceship Crew Sizes**
- This bar chart displays the number of crew members required for each spaceship, helping users compare their capacities.
3. **Character Analysis**
- Graph of character heights and weights
4. **Planet Analysis**
- Scatter plot of planets by population.
5. **Starships Comparison**
- Bar chart comparing starship capabilities.


## License
© Copyright 2015, Paul Hallett. Revision cb9195fc.
All rights reserved.
Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
* Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
* Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
* Neither the name of swapi nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE. (Referense: https://github.com/semperry/swapi/blob/master/LICENSE)

## Acknowledgments
- [SWAPI](https://swapi.dev/) for providing the Star Wars API.

