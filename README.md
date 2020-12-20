# Snowman Weather App

GITHUB LINK
TRELLO BOARD LINK
SLIDE DECK LINK

### Purpose
Snowman Weather app is Weather application written in Ruby for terminal which will give you options to find out weather for today, tomorrow, and 5 days (weather api). City lists will be also uploaded through OpenWeather Ruby Client (link)
https://github.com/dblock/open-weather-ruby-client

There are various apps over there and I wanted to make a version of the weather app that would be interactive and would create interaction of a snowman depending on weather forecast. 
Who might be interested in this?

I belive that this app might be interesting for anyone who is searching for weather forecast. And if they find out about life of a snowman - that is definitely a bonus. When snowman gets ascii images and the app passes condition statements for snowman, it will be quite fun and kids might enjoy it as well: it is a way to learn what happens to snowman in different types of weather.

### Features


## Diagram

![Alt text here](images/someimage.png)

## 

## Requirements

## Extras

## Implementation plan

17-18 Dec 2020
For a few days I have been reasearching ways how to implement weather api for my application. As I came across OpenWeather API, I was planning to use it normal way at the beginning. However then I came across OpenWeather Ruby Client and decided to use that one. It seemed to be much simpler to implement this data and it was more straighforward. I managed to run a few error tests and now if the input of city and country don't match in the exsting list of countries and cities, it returns an error message.

CODE insert!!!!!!!!

19 Dec 6 pm
After receiving commentary from teachers based on my presentation, I decided to focus on the mvp and make sure that the core application runs without implementing major sprinkles.

20 Dec 2 pm
After consulting educators, I needed to save my api_key in external file and then parse it to the main file. I ran a few tests in a separate file and it returned the required key to me, however it didn't run in the main file. I would appreciate to get some commentary on the best way to parse it to the index.rb file so I know for the future.

20 Dec 6 pm
I had to refactor ascii images of the snowman as I couldn't sort out how ascii art gem works
Now focusing on filling in documnetation.

20 Dec 7 pm
Working on command line arguments
- help
- version
![Command-line-argument](../docs/screenshots/terminal arguments Screen Shot 2020-12-20 at 8.05.33 pm.png)

## Testing
## Backlog
I sat down and refactored some of the donut/sprinkles requirements within my Trello board. Animation stayed as a backlog sprinkle and ascii images of snowman has been downgraded to sprinkle. I will try to implement those after submitting my application. 
Not complete:
- [x] animation (not complete)
- [x] ascii images of snowman
https://www.rubydoc.info/gems/ascii-image/0.1.2/ASCII_Image 

## Help Documentation


### Steps to install application

### Dependencies required to operate
### System requirements

