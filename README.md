# friendFinder
Week 7 homework 2




Friend Finder App.  Find your TRUE friend.

## Live Link 
 - (https://finderoffriend.herokuapp.com/)

## Usage

![website screenshot](https://github.com/mra-abrahamson/friendFinder/blob/master/mysocialnetwork.PNG)

Go to our homepage and take our survey. After submitting the survey, your TRUE friend will appear. 


## Technologies Used

- JavaScript
- jQuery
- node.js
- Express.js
- HTML
- Bootstrap
- Heroku

## Code Explanation
- Our `server.js` file sets up the Express server, specifying our port number, the npm packages that need to be loaded, and also the routes, which we have externalized
- There are 2 separate HTML files (`home.html` and `survey.html`) that serve as the front-end portion of our code; they determine what the user sees (the homepage and the survey, which will also show the resulting best match)
- Our 2 routing files (`htmlRoutes.js` and `apiRoutes.js`) determine the back-end logic (based on the request being made, the response that gets sent to the browser); the HTML routes display the survey and the homepage based on the URL that is accessed, and the API routes send back existing content in our server-side data or add new friends
- Best match is calculated by finding the friend with the minimal difference in scores and then sending that friend to the browser as a JSON object
- A modal is then toggled, displaying the the best match to the person who just took the survey
- In essense, this will also be a form of notes that you may later reference weeks later
- Friends are stored as such:

```js
{
	name: "Precious",
		photo: "https://goo.gl/images/Pdpjbs",
		scores: [1, 1, 5, 3, 3, 5, 1, 2, 5, 4]
}
```
