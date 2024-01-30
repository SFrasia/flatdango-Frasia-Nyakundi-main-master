# Flatdango Project

![Screen Shot 2024-01-30 at 9 46 51 PM](https://github.com/SFrasia/flatdango-Frasia-Nyakundi-main-master/assets/108404961/2d5f2dd5-7805-4583-9279-184969669ec0)

## Table of Contents

- [Overview](#overview)
- [Getting Started](#getting-started)
- [Core Deliverables](#Coredeliverables)
- [License](#license)

## Overview

For this assessment, you'll be working on Flatdango.
Flatiron Movie Theater is open for business! You will be building out an application, Flatdango, that allows a user to purchase movie tickets from the theater.

The instructions below will walk you through the process of ideation and planning your app: deciding on your user interface, planning how the information will be laid out on the page, etc. You should work through all the planning steps before you start doing any coding.

## Getting Started

1. Download the server db.json file from here `Download here`
2. Ensure you have `json-server` installed on your machine.
3. Run this command to get the backend started: `$ json-server --watch db.json`
4. Test your server by visiting this route in the browser: `http://localhost:3000/films`

## Core Deliverables

As a user, I can:

See the first movie's details, including its **poster, title, runtime,
   showtime, and available tickets** when the page loads. The number of

   available tickets will need to be derived by subtracting the number of

   `tickets_sold` from the theater's `capacity`. You will need to make a GET

   request to the following endpoint to retrieve the film data:

  

   GET /films/1

   Example Response:

   {

     "id": "1",

     "title": "The Giant Gila Monster",

     "runtime": "108",

     "capacity": 30,

     "showtime": "04:00PM",

     "tickets_sold": 27,

     "description": "A giant lizard terrorizes a rural Texas community and a heroic teenager attempts to destroy the creature.",

     "poster": "https://www.gstatic.com/tv/thumb/v22vodart/2157/p2157_v_v8_ab.jpg"

   }

See a menu of all movies on the left side of the page in the `ul#films` element when the page loads. (_optional_: you can style each film in the list by adding the classes `film item` to each `li` element.) There is a placeholder `li` in the `ul#films` element that is hardcoded in the HTML — feel free to remove that element by editing the HTML file directly, or use JavaScript to remove the placeholder element before populating the list. You will need to make a GET request to the following endpoint to retrieve the film data:

   GET /films

   Example response:

   [

      {

        "id": "1",

        "title": "The Giant Gila Monster",

        "runtime": "108",

        "capacity": 30,

        "showtime": "04:00PM",

        "tickets_sold": 27,

        "description": "A giant lizard terrorizes a rural Texas community and a heroic teenager attempts to destroy the creature.",

        "poster": "https://www.gstatic.com/tv/thumb/v22vodart/2157/p2157_v_v8_ab.jpg"

      },

      {

        "id": "2",

        "title": "Manos: The Hands Of Fate",

        "runtime": "118",

        "capacity": 50,

        "showtime": "06:45PM",

        "tickets_sold": 44,

        "description": "A family gets lost on the road and stumbles upon a hidden, underground, devil-worshiping cult led by the fearsome Master and his servant Torgo.",

        "poster": "https://www.gstatic.com/tv/thumb/v22vodart/47781/p47781_v_v8_ac.jpg"

      }

   ]

Buy a ticket for a movie. After clicking the "Buy Ticket" button, I should see the number of available tickets decreasing on the frontend. I should not be able to buy a ticket if the showing is sold out (if there are 0 tickets available). **No persistence is needed for this feature**.


## License
This project is licensed under the `Moringa School.`

