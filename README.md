# Covid Vaccine Tracker for United States

Covid Vaccine Tracker(CVT) is a React website built for the purpose of tracking the progress of vaccinations within the United States and its territories. This website was built with React and Material UI.

View live site [here](https://covid-vaccine-tracker-us.herokuapp.com/). 
- Quick discislaimer this website is stored on a Heroku store. So it may take a bit before it wakes up.

## Process

* Parsed csv data provided by [Our World in Data](https://ourworldindata.org/).
* Saved latest entries from csv to React state.
* Display chosen locations vaccine data from csv when user selects from a drop down.
* Data displayed will show amount of people who received one dose, amount of people fully vaccinated(according to manufacturer  guidelines), and percent of population fully vaccinated.

## Installation

1. Clone github repo
2. Change directory to client.
    ```
    $ cd client
    ```
3. Run npm install.
    ``` 
    $ npm install
    ```
4. After install run npm start.
    ```
    $ npm start
    ```
5. Navigate to localhost:3000 in your web browser

## Docker Install

1. Build the container image. 
    ```
    $ docker build -t {name_of_image} .
    ```

2. Start a new container. 
    ```
    $ docker run -dp 3000:3000 --name covid_tracker_container {name_of_image}
    ```

3. Open browser to localhost:3000.

## Roadmap 

Rely solely on material UI, and keep external styling to a minimum.
Possible socket implementation with live updates.
