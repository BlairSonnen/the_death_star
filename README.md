# Star Wars API Project

## Overview
The Star Wars API Project is a web application that enables users to explore data from the Star Wars universe by interacting with the Star Wars API (SWAPI). The project focuses on gathering information about spaceships and characters, allowing users to analyze the data and visualize it through graphs. This project aims to provide insights into various attributes of Star Wars entities.

## Features and Usage
- Retrieve and display information on various Star Wars spaceships and characters from the SWAPI.
- Collect user preferences to create a new DataFrame for analysis.
- Generate visualizations (e.g., bar charts, scatter plots) to analyze relationships between different attributes (e.g., ship speeds, character heights).
- Easy-to-use interface for searching and selecting specific spaceships and characters.

## Technologies Used
- Fetch API for interacting with SWAPI root:
https://www.swapi.tech/api/
- Data manipulation with Python 
- Pandas, Json, Numpy, Urllib.request, Matplotlib.pyplot

## Data Collection
Users can collect data by selecting the following:
- Spaceships: Users can choose from a list that includes starship names, speeds, and crew sizes.
- Characters: Users can select character details such as names, heights, weights, and homeworlds.
The selected data is used to create a new DataFrame for further analysis and visualization.

### Example Data Collection Process:
1. A user selects a spaceship and one or more characters.
2. The application retrieves and stores the selected data into a structured format (e.g., an array of objects).
3. This data is transformed into a DataFrame, where each entry corresponds to a spaceship and the associated character(s).

## Data Analysis and Visualization
After data collection, the project analyzes relationships between different attributes of the selected spaceships and characters. Users can visualize:
- **Spaceship Speeds** vs. **Character Heights**: A scatter plot to explore any correlation between these two metrics.
- **Crew Size of Spaceships**: A bar chart showing the number of crew members per spaceship.

### Visualization Examples:
1. **Scatter Plot of Spaceship Speeds vs Character Heights**
- This graph illustrates whether there's a significant correlation between the speed of the ships and the heights of characters.
2. **Bar Chart of Spaceship Crew Sizes**
- This bar chart displays the number of crew members required for each spaceship, helping users compare their capacities.
3. **Character Analysis**
- Graph of top 10 characters by film appearances.
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

