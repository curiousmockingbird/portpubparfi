# Portland Public Party Finder

#### Created by Harold Mesa, Kelly Bruce, Helen Lehrer, Tiberius Lockett , and Noah Lundquist in September of 2022

## Links

* [Repository](https://github.com/curiousmockingbird/portpubparfi)

## Description

Group project working with social media APIs to find events by categories in the greater Multnomah County area. 

## Features

* Calls upon EventBrite and PredictHQ APIs.  
* Filters results by categories.

## Technologies Used

* Built in VS Code (v.1.70.1) using the following languages:
	* HTML
	* CSS
	* Javascript
  * Bootstrap

* Packages used include:
	* Webpack
	* ESLint
	* Babel
	* Jest

* Tested in the following browsers:
	* Google Chrome (v.104.0)


## Installation

* Download [Git Bash](https://git-scm.com/downloads)
* Input the following into Git Bash to clone this repository onto your computer:

		>git clone https://github.com/curiousmockingbird/portpubparfi

* Enter the cloned project folder "portpubparfi" and type:

		>npm install

* After such you can type the following command to host the site on your machine at localhost:8080 :

		>npm run start

The EventBrite API functionality will _not_ be available until you do the following:

* [Sign up or Log into](https://www.eventbrite.com/signin/?referrer=%2Fplatform%2Fapi) Eventbrite and visit your API Keys page. 
* Copy your private token.
* Create a .env file in the root of the "portpubparfi" folder
* Open the .env file in VS Code or the editor of your choice and input:  
BEARER_TOKEN_EB=[your EventBrite bearer-token here]

The PredictHQ API functionality will _not_ be available until you do the following:

* [Sign up or Log into](https://auth.predicthq.com/login?continue=https%3A%2F%2Fauth.predicthq.com%2Fauthorize%3Fresponse_type%3Dcode%26client_id%3Dcontrol_client%26scope%3Dusers%253Aread%2Bmemberships%253Aread%2Buser-profiles%253Aread%26redirect_uri%3Dhttps%253A%252F%252Fcontrol.predicthq.com%252Fauth%252Flogin%26state%3D4x3nuvyewa5) PredictHQ and visit your API Keys page. 
* Copy your private token.
* Create a .env file in the root of the "portpubparfi" folder.
* Open the .env file in VS Code or the editor of your choice and input:  
BEARER_TOKEN_LE=[your PredictHq bearer-token here]  
ACCESS_TOKEN=[your PredictHq access-token here]  
ACCESS_TOKEN_SECRET=[your PredictHq access-token-secret here]  
API_KEY=[your PredictHq API-key here]  

## Known Bugs

* We have experimental branches for Facebook & Twitter APIs that are not functional due to authentification errors.
* In the UI, when the height of the viewport changes size, the event result div superimposes onto the blue form div.
* There is overflow text for the results of the PredictHQ API, so there is currently a scroll bar at the bottom of the column to account for that.
* The Eventbrite events have to manually updated becasue the API doesn't allow for dynamic search capability.

## License

Licensed under [GNU GPL 3.0](https://www.gnu.org/licenses/gpl-3.0.en.html)

Test #1
