# Weather App
#### Video Demo:  <https://www.youtube.com/watch?v=7yTaVZs0FG0>
#### Description:

the program demonstrates a simple weather app which displays 3 things:
Humidity, Wind Speed, and the Weather in Fahrenheit

First the user has to enter any city name to get the data for weather and
the icon changes as the weather changes.

If the city is entered in wrong the program complains that there is an *invalid input* and asks the user
to enter another city

The program derives its city information from an API which stores a large amount of information on the weather of cities around the world

this is the link to the API: <https://openweathermap.org/api/one-call-3>

Additionally, I used images to change the icons, I have also attached files to those images in this project

I used JavaScript, CSS and HTML to make this project, it was a simple use of API and basic code that we have learned from this course



## CODE

Here is some of my `css`

```css
.card{
    width:90%;
    max-width: 470px;
    background: linear-gradient(135deg, #00feba,#5b548a);
    color: #fff;
    margin:100px auto 0;
    border-radius: 20px;
    padding: 40px 35px;
    text-align: center;
}
    //I also used margin, align items and justify content
```

This is how I grabbed data from a database I found online with accurate weather information

```js
const apiKey = "6e55e4f908c8f5e1d622161c5a3213ec";
const apiUrl = "https://api.openweathermap.org/data/2.5/weather?units=imperial&q=";

const searchBox = document.querySelector(".search input");
const searchBtn = document.querySelector(".search button");
const weatherIcon = document.querySelector(".weather-icon");
```

I also had to use inspect on my local server and look at console logs to grab certain data from the API
Below is the `code` for that

```js

    document.querySelector(".city").innerHTML = data.name;
    document.querySelector(".temp").innerHTML = Math.round(data.main.temp) + "°F";
    document.querySelector(".humidity").innerHTML = data.main.humidity + "%";
    document.querySelector(".wind").innerHTML = Math.round(data.wind.speed) + " mph";
```

based on what the API data described the weather as I included certain images to representy clouds, mist and rain etc

## LINKS

[API Source](https://openweathermap.org/api)

[HTML/CSS "cheatsheet"](https://htmlcheatsheet.com/css/)

## CSS features used and their uses

| Feature | Description |
| ------ | ----------- |
| Box-sizing   | allows us to include the padding and border in an element's total width and height|
| Border-radius | allows us to round the corners of a circular object |
| Justify-content | allows us to define how the browser distributes space between and around content items along the main-axis of a flex . |
| flex | allows us to set how a flex item will grow or shrink to fit the space available in its flex container. |
| display | allows to specify how an element is shown on a web page |




### Why I chose this project

I wanted to do something simple using a topic I enjoyed, I personally liked the combination of HTML, JS and CSS and so I decided to make a program using that combination. I find CSS and HTML really fun, and weather is an everyday need. After packaging the site I will be able to add the site to my home page to my phone and use my own site on the daily, and I find that a very strong incentive to create this as a simple final project to reflect what I learned from CS50 and the self learning I did to craft this project
