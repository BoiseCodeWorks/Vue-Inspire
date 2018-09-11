# Foundations - Vue-Inspire
Inspiration can be difficult to achieve. Keep track of your many important tasks and the weather with the suttle help of a random daily quote and beatiful scenery.   

## The Setup
This will be a Vue based project. It will be up to you to determine what components to use, and when to use them.

### Front-End
This time around you are creating the project and files as well as the basic structure. Take some time to think about how you want to layout your project and ultimately how it will function. Remember utilizing unidrectional data flow patterns for getting and maintaining the data integrity. A vuex store utilizing actions and mutations to get and set our data to keep our data true across components.

After setting up the basic html structure and methods in your components, you will be responsible to connect each of the components to the appropiate actions in your store. Be aware of what a component needs to gain access to the needed methods and data residing in the store.

Your goal will be to put all of the requests, and data gathered from them, together in a visually pleasing format as well as ensuring the functionality of a todo list. 

Below you will see an image that you may use for inspiration. 

<div class="text-center">
    <img class="img-responsive" src="https://bcw.blob.core.windows.net/public/img/inspire.jpg"/>
</div>

### Adding the functionality 

The todolist is perhaps one of the most important features of this application. You will need to provide the user a way to add items to a list to be monitored for tracking. The user should be able to add or remove items easily as well as be able to indicate an items status if they don't want to remove the item(completed). Use Firestore to persist data.

### Prettify

You can use the picture above as an idea for laying out your site. One of the main goals of this project is to have a final portfolio piece that displays well. It is the final accumulation of all of your abilities to produce something with both excellent functionality and an aesthetically pleasing user interface.

## The API

### Todo model Example
```javascript
{
    name: { type String, required: true}                            //has to be a string
    description: { type: String, required: true},                   //has to be a string
    completed: { type: Boolean, required: true, default: false},    //has to be a bool
    userId: {type: ObjectId, ref: 'User'}                           //has to be a users id
}
```

## Other Requests

### Image Request
http://bcw-sandbox.herokuapp.com/api/images - retrieves a random image

### Quote Request
http://bcw-sandbox.herokuapp.com/api/quotes - retrieves a random quote

### Weather Request
http://bcw-sandbox.herokuapp.com/api/weather - retrieves the weather


### EXTENSION IDEAS 
- On hover the quote should show the author of the quote and disappear when not hovered over
- A clock should be rendered to the screen that updates each minute without a page refresh
- Allow the user to set their name and have it save to localStorage
- Change the message from Good Morning to Good Afternoon, Evening as appropriate. 
- Allow the user to toggle the clock from, 12hr to military time. 
- Include an Icon to show what the weather is sunny/cloudy/rainy
- Add a button to cycle to next quote/picture
- Could you encorporate a deadline for some of the tasks
- Add a settings so user can change to a new "theme" (font, background colors, etc.)
- Clicking the weather should let the user toggle between Celsius, Fahrenheit, or even Kelvin display
- Todo list slides away to the side of the screen
- The todolist shows the total count of tasks currently being tracked
- Utilize an external vue component for the clock or weather
- Use an image, weather, or picture API of your choice
- Add Itunes or another music API to the app

## REQUIREMENTS:
 - Visualization
   - The data from Quote, Image, Weather, and Todo are each rendered.
   - The image should be on large display with at least one other element positioned over the top of the image.
 - Functionality
    - The todolist allows items to be added and removed from a list
    - The todolist takes advantage of the Todo API request to provide persistent data through our database Server

### Finished?
When You are finished please deploy and submit the link to the project in the backpack.
