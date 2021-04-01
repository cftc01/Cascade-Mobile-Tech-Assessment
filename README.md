# Technical Assessment
NOTE: All work for this position is done using Swift and various iOS libraries and frameworks.

## Overview
This exercise is intended to take no longer than 4 hours.  Please limit the detail of your solution with that time in mind.  Please include a README with your submission detailing your solution.

## Problem
Lets assume Cascade Fintech has contracted you to build a **Feature** prototype to support purchasing Pokemon.  

## Data definition

The following is a snippet of the data you would recieve using the PokeAPI https://pokeapi.co/

Using the API as a data source create an app that takes the name of a Pokemon and tells the user if they have sufficient funds to purchase that Pokemon. 

The purchase price for a Pokemon will be 1% of the base_experience X 6. Using the example above you should get $14.40

```json
  "abilities": [
    {
      "ability": {
        "name": "blaze",
        "url": "https://pokeapi.co/api/v2/ability/66/"
      },
      "is_hidden": false,
      "slot": 1
    },
    {
      "ability": {
        "name": "solar-power",
        "url": "https://pokeapi.co/api/v2/ability/94/"
      },
      "is_hidden": true,
      "slot": 3
    }
  ],
  "base_experience": 240,
  "forms": [
    {
      "name": "charizard",
      "url": "https://pokeapi.co/api/v2/pokemon-form/6/"
    }
  ],
  "game_indices": [
    {
      "game_index": 180,
      "version": {
        "name": "red",
        "url": "https://pokeapi.co/api/v2/version/1/"
      }
    },
    {
      "game_index": 180,
      "version": {
        "name": "blue",
        "url": "https://pokeapi.co/api/v2/version/2/"
      }
    },
```

Your app should satisfy the following:
- Allow the user to enter a Pokemon name
- If the name does not exist an error message should be displayed to the user
- If the user can purchase the Pokemon he should be greeted with a screen that shows the user summary of the purchase and a complete the purchase buttont that is not connected to anything. 
- If the user cannot purchase the Pokemon they should be made aware they do not have sufficient funds to purchase the Pokemon.

Hint: Think of yourself as the user, what information do you need to know about the current status of your account below you will find a sample user profile.

```json
"user": {
  "name": "",
  "last": "",
  "accountNumber": 11133344556433443,
  "balance": 12.34,
  "email": "someuser@thedomain.com"
	}
```

___

## Submission
- Send an email to your Cascade contact with a link to your solution on your github account when completed.

Do not submit a PR. 
Do not ask for external assistance. 
Do not share solution or assessment with outside sources.
