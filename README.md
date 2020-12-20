# Snowman Weather App

[GITHUB LINK](https://github.com/iri6ka/snowman_weather_app)

[TRELLO BOARD](https://trello.com/b/K0z1wQ5F/snowman-weather-app)

[SLIDE DECK](https://docs.google.com/presentation/d/1TiodhFck0bXgd9WnrGsd4DLVyNx5QTGorSmvxqasXoE/edit?usp=sharing)

### Purpose
Snowman Weather app is Weather application written in Ruby for terminal which will give you options to find out weather for today, tomorrow, and 5 days (weather api). City lists will be also uploaded through [OpenWeather Ruby Client](https://github.com/dblock/open-weather-ruby-client)

##### Reason
I decided to develop this app as it was intersting to me how developers are working with various api. As I was going through research, I found various api applications and especially weather applications. It was important for me as for a junior developer to understand the methods and calls behind api calls and the whole journey was quite challenging but very rewarding as I finally figured out how to use it.

##### Market & Usage
There are various apps over there and I wanted to make a version of the weather app that would be interactive and would create interaction of a snowman depending on weather forecast. The current version of the application is a variation of minimal viable product, but it is important to have an understanding that mvp is working correctly before implementing 'sprinkles' and adding various new features.

I belive that this app might be interesting for anyone who is searching for weather forecast. And if they find out about life of a snowman - that is definitely a bonus. When snowman gets ascii images and the app passes condition statements for snowman, it will be quite fun and kids might enjoy it as well: it is a way to learn what happens to snowman in different types of weather.

#### Application scope
Snowman Weather Application is supposed to interact with the user the following way: it asks the user for name, then uses name as a way to address to the user, asks for user city and country and then based on those variables calls OpenWeather Api and returns output with various weather components: current temperature, feels like, minimum and maximum weather for the day. In the future the app will also provide update on the life of a snowman - how his state changes depending on current temperature of the day. The app will also show the user the way how the snowman changes depending on the temperature.

### Features

Application contains 3 main features.
1. Weather api. Through Open Weather Ruby client I was able to make api call to OpenWeather website and request weather data from their database. At the moment it calls for the following data.
2. Snowman Weather app uses `ascii art` (`$ artii gem`) to process text into `ascii` art.
3. The app is reading external txt files. At the moment the app uses `installation.txt` file in order to show what are the minimal requirements to run this application.
4. Minimal animation
At the end of the program once user selected option to quit, the terminal asks to enter any key and then puts `*****` with animation, and then puts `'Goodbye'`.

Examples:
![Example1](https://github.com/iri6ka/snowman_weather_app/blob/old-project/docs/screenshots/ascii%20name.png)
![Example2](https://github.com/iri6ka/snowman_weather_app/blob/old-project/docs/screenshots/help%20file.png)

## Diagram

![Link](../docs/Diagram.png)

## Trello
![](../docs/screenshots/trello 2.png?raw=true)

![](../docs/screenshots/Trello 3.png?raw=true)

![](../docs/screenshots/Trello 4.png?raw=true)

![](../docs/screenshots/trello 5.png?raw=true)

![](../docs/screenshots/Trello 6.png?raw=true)

![](../docs/screenshots/Trello 7.png?raw=true)

## Implementation plan

*15-16 Dec 2020*
Initial research on the application, idea on what the application might be.

*17-18 Dec 2020*
For a few days I have been reasearching ways how to implement weather api for my application. As I came across OpenWeather API, I was planning to use it normal way at the beginning. However then I came across OpenWeather Ruby Client and decided to use that one. It seemed to be much simpler to implement this data and it was more straighforward. I managed to run a few error tests and now if the input of city and country don't match in the exsting list of countries and cities, it returns an error message.

Trello board creation.

*19 Dec 6 pm*
After receiving commentary from teachers based on my presentation, I decided to focus on the mvp and make sure that the core application runs without implementing major sprinkles.

*20 Dec 2 pm*
After consulting educators, I needed to save my api_key in external file and then parse it to the main file. I ran a few tests in a separate file and it returned the required key to me, however it didn't run in the main file. I would appreciate to get some commentary on the best way to parse it to the index.rb file so I know for the future.

*20 Dec 6 pm*
I had to refactor ascii images of the snowman as I couldn't sort out how ascii art gem works
Now focusing on filling in documnetation.

*20 Dec 7 pm*
Working on command line arguments
- help
- version
![](https://github.com/iri6ka/snowman_weather_app/blob/old-project/docs/screenshots/terminal%20arguments%20Screen%20Shot%202020-12-20%20at%208.05.33%20pm.png?raw=true)

## Testing

There are a few tests running throughout the app. 
Wrong input of city and country. If city and country don't exist, then the user gets error messages. A few other wrong inputs within the app give error messages.
![Error1](https://github.com/iri6ka/snowman_weather_app/blob/old-project/docs/screenshots/Error%20handline%202.png?raw=true)
![Error2](../docs/screenshots/error handling 1.png)
![Error2](../docs/screenshots/error handling 2.png)
![Error2](../docs/screenshots/error handling 3.png)
![Error2](../docs/screenshots/error handling 4.png)
![Error2](../docs/screenshots/error handling 5.png)
![Error2](../docs/screenshots/error handling 6.png)
![Error2](../docs/screenshots/error handling 7.png)



## Backlog
I sat down and refactored some of the donut/sprinkles requirements within my Trello board. Animation stayed as a backlog sprinkle and ascii images of snowman has been downgraded to sprinkle. I will try to implement those after submitting my application. 
Not complete:
- [x] animation (partially complete)
- [x] ascii images of snowman (not complete)
[Link](https://www.rubydoc.info/gems/ascii-image/0.1.2/ASCII_Image)

## Help Documentation and System requirements

In order to run the file properly, it is possible to require -help through terminal while putting
`$ ruby index.rb -help`. File explaines on the system requirements, dependencies required to run application and show steps how to run the file.

The terminal will open text file with the following:
```
To run Weather Snowman App you would need to install the following:

1. Ruby ~version 2.7.1p83 or higher. Make sure that you are using rvm or a preferred ruby version manager
2. Enruse that you are running Ruby ~version 2.7.1p83.
3. Install the following GEMS:
    a) install bundler ($ gem install bundler)
    - $ bundle install
    b) install tty-prompt ($ gem install tty-prompt)
    c) install httparty ($ gem install httparty)
    d) install artii ($ (sudo) gem install artii)
    e) install colorize ($ install gem colorize)
    f) add OpenWeather Ruby Client to Gemfile ($ gem 'open-weather-ruby-client'). Then run bundle install.
4. Run ruby index.rb
Enjoy!

```
**Gem** dependencies can be found through Gemfile & Gemfile.lock

### Code

![Example1](../docs/screenshots/code 1.png)
![Example2](../docs/screenshots/code 2.png)
![Example3](../docs/screenshots/code 3.png)
![Example4](../docs/screenshots/code 4.png)
![Example5](../docs/screenshots/code 5.png)
![Example6](../docs/screenshots/code 6.png)
![Example7](../docs/screenshots/code 7.png)
