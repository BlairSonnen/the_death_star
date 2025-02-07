
## Overview
The Star Wars API Project is a web application that enables users to explore data from the Star Wars universe by interacting with the Star Wars API (SWAPI). The project focuses on gathering information about the user's character preference, allowing users to compare the selected character data against the rest of the Star Wars world, and visualize it through graphs. This project aims to provide insights into various attributes of Star Wars entities.

## Source Information and Installation

API base URL: https://swapi.dev

- People: 82 rows X 16 columns
- Planets: 60 rows X 14 columns
- Films: 6 rows X 14 columns
- Species: 37 rows X 15 columns
- Vehicles: 39 rows X 16 columns
- Starships: 36 rows X 18 columns

### Installations necessary dependencies

Clone this repository:
```
git clone <repository_url>
```
Then install:
```
pip install asyncio
pip install aiohttp
pip install ipywidgets
```
### Run the Jupyter Noteboox
```
jupyter notebook star_wars.ipynb
```

## Features
- People: name	height	mass	hair_color	skin_color	eye_color	birth_year	gender	homeworld	films	species	vehicles	starships	created	edited	url
- Planets: name	rotation_period	orbital_period	diameter	climate	gravity	terrain	surface_water	population	residents	films	created	edited	url
- Films: title	episode_id	opening_crawl	director	producer	release_date	characters	planets	starships	vehicles	species	created	edited	url
- Species: name	classification	designation	average_height	skin_colors	hair_colors	eye_colors	average_lifespan	homeworld	language	people	films	created	edited	url
- Vehicles: name	model	manufacturer	cost_in_credits	length	max_atmosphering_speed	crew	passengers	cargo_capacity	consumables	vehicle_class	pilots	films	created	edited	url
- Starships: name	model	manufacturer	cost_in_credits	length	max_atmosphering_speed	crew	passengers	cargo_capacity	consumables	hyperdrive_rating	MGLT	starship_class	pilots	films	created	edited	url

## Data Cleaning
- Converted all non-male and non-female entires to non-binary
- Convert height and mass columns to int type from object. Verified with basic statistics.
- Created a function that categorizes character mass into ranges: '0-50', '51-100', 'Over 100'
- Clean up species data that is stored as empty arrays.
- Clean up the classification column to convert reptilian to reptile and mammals to mammal.
- Created a function to retrieve all information from the other dataframes based on the person's homeworld, species, starships, and vehicles. 

## Exploratory Data Analysis (EDA)
- Retrieve and display a plot of character height sorted from shortest to tallest and highlight selected character.
<img width="1185" alt="Screenshot 2025-02-06 at 10 59 53 AM" src="https://github.com/user-attachments/assets/a54f9765-f4f6-4ef0-8c03-987d44fda2ef" /># Star Wars API Project

Other retrieve and plot display examples from the SWAPI.
- Character Mass
- Surface Water Percentage by Planet
- Population Density by Planet, and same plot with Log10 scale
- Lifespan by Species
- Starship Cost
- Starship Capacity
- Film Count by Character, Planet, Species, Starship
- The user will start their journey in this world by being asked:"What character would you like to be today?"
- They will then be presented with a list of character genders to select from
- After that selection, they will be asked what hair color will want (from a list of remaining options)
- And finally, they will be asked what eye color they want (from a list of remaining options)

## Usage
Running the application will result in the following display.

<img width="693" alt="Screenshot 2025-02-06 at 11 11 29 AM" src="https://github.com/user-attachments/assets/c3e7068d-57f3-4072-8e4d-5d2811d3f716" />

1. A user selects a character through a question and answer process.
   Users can select character details such as gender, species, and mass range.
3. The application retrieves and stores the selected data into a structured format (e.g., an array of objects).
4. This data is transformed into a DataFrame, where each entry corresponds to a spaceship and the associated character(s).

The result will then store the selected character for comaprison analysis to the rest of the Star Wars ecosystem and generate visualizations (e.g., bar charts, scatter plots) to analyze relationships between different attributes examples: 

* Characters - Height, Mass comparisons
* Home world - Diameter, Population comparisons
* Species - Life span, Height comparisons
* Starships - Speed, Capacity comparisons

### Visualization Examples:

1. **Bar Chart of Character Height**
- This bar chart displays the height of all characters as compared to the selected character.
<img width="865" alt="Screenshot 2025-02-06 at 11 32 47 AM" src="https://github.com/user-attachments/assets/2a42df13-d6d5-4115-9e7e-35596a5f3871" />


# An Easy-to-use interface for searching and selecting specific characters and learning how their information compares to the rest of the Star Wars ecosystem.




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
- Star Wars and all associated names are copyright Lucasfilm ltd.

