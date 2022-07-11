## Full cycle used car price prediction (from scrapping to moddeling)

#### Steps taken
I chose to work with the autotrader.com website to try to gently extract data of about 150 thousand vehicles all over the US. Figuring out the url logic of the website I have created the *url = core_link + car + make + end_link + pagination + str(page)* where core linke gives *https://www.autotrader.com/cars-for-sale/*, car variable choses either new or used car, end link includes all the information about the zip code, distance and other parameters, pagination includes how many vehicles to show and wich page to be on.

The initial apporach with requests library did not yield me any results with *Autotrader - page unavailable*, eventhough the generated links copied directly into the web browser opened corresponding pages.

This is where I decided to explore other options, namely vast number of available APIs.

