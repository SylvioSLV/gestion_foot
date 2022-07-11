# gestion_foot

# API REST pour la gestion des statistiques des joueurs de foot de l'équipe nationale du Togo.

# Project for the occasion of D-CLIC Program just for build and deploy this API on [Heroku Website.](https://id.heroku.com/login)

# Tools used to build the API :

- NodeJS 
- Express.js – Fast, unopinionated, minimalist web framework for [Node.JS](https://nodejs.org/en/)

# Packages installed :
- nvm – Node Version Manager
- npm – Node Package Manager
- Node.js
- Express installed with npm *(npm install express body-parser morgan).*

# How to Use : 
- POST https://safe-fjord-52502.herokuapp.com/api/v1/stats

    - This will create the stats a player

        // this is the input examples
            {
                "id": 20,
                "wins": 0,
                "losses": 10,
                "points_scored": 0
            }
        // and it will return json file like this
            {
                "id": 20,
                "wins": 0,
                "losses": 10,
                "points_scored": 0
            }

- GET https://safe-fjord-52502.herokuapp.com/api/v1/stats/20

    - This will get the stats for player 20

        // it will return json file like this
            {
                "id": 20,
                "wins": 0,
                "losses": 10,
                "points_scored": 0
            }

- PUT https://safe-fjord-52502.herokuapp.com/api/v1/stats/20

    - This will update the stats for player 20

        // this the input 
            {
                "id": 20,
                "wins": 2,
                "losses": 1,
                "points_scored": 4
            }
        
         // and it will return json file like this

            {
                "id": 20,
                "wins": 2,
                "losses": 1,
                "points_scored": 4
            }

- DELETE https://safe-fjord-52502.herokuapp.com/api/v1/stats/101

    - This will delete the stats for player 101

        // this the input 
            {
                "id": 101,
                "wins": 10,
                "losses": 3,
                "points_scored": 7
            }

        // and it will return an empty json file
