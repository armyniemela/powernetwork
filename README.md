# Project02: Power network
This is my fourth assignment in Lede, where I create a webpage. Project02 is called Power Network and it's about a familiar topic to me: it involves handling one of my job tasks in a different way. Arvopaperi magazine, where I work as a subeditor, conducts the "Network of Influence" survey annually on the board members and CEOs of publicly traded companies in Finland. We have not been able to create a visualization from the data that shows the network of individuals and companies interactively. My goal here was to create such a visualization using a new viztool for me. Additionally, I wanted to process the original data in a notebook using pandas, as I have done it in Excel for many years.

## Sources and data collection for Power network
I had access to the data collected for the Arvopaperi article in Excel format. It contained about 2000 of rows and 20 of columns of information about the board members of companies listed on the Helsinki Stock Exchange. The formulas for the market values of the companies were already prepared from the stock values. I used these market values, even though they were collected in the spring so some are incorrect now but not different in scale. 

Additionally, for some reason, the data included only 136 companies, and I couldn't determine why some publicly traded companies were missing. I verified that the number of publicly traded companies is 180, excluding different share series and combining shares on [OMX Helsinki](https://www.kauppalehti.fi/porssi/indeksit/OMXHPI) and [OMX First North](https://www.kauppalehti.fi/porssi/indeksit/FNFIEURPI). One reason for the different amount is that there have been new listings and stock mergers, but the number suggests that the original data was limited. The data was originally collected by Alma Business Media's information service.

Compared to the original Network of Influence, I used the entire dataset, whereas the material for the Arvopaperi article was immediately limited to those with networks, meaning those with 2 or more board seats. In my project, the CEOs of the companies are not considered.

Here is a link to [Arvopaperi's article](https://www.arvopaperi.fi/uutiset/tallainen-on-helsingin-porssin-vallan-verkosto-risto-murto-vahtii-viidesosaa-porssin-markkina-arvosta-arja-talma-47-7-miljardia-euroa/c48e0689-2410-4b32-8eb5-a84c53971bdb). I also want to give a shout out to Silva Rehn and KP Alare. Rehn wrote the article and Alare and I worked on the viz together.


## Pandas work for Power network
The project required a lot of preliminary work in Jupyter Notebook with Pandas. One of the goals of the project was to become proficient with Pandas, and this was achieved successfully.

Firstly, I created three different types of graphics, each requiring slightly different data. At first, I didn't know which values needed to be arranged and how, since I had never created an SVG-D3 graphic before. Also the other types of graphs and Flourish were new to me. Secondly, the dataset contained a lot of inconsistencies. It would have been easier if Jeremy's Tidy Data lecture was before I started... 

The great thing was that I was much more efficient in summarizing the data for this project than when working on the Arvopaperi article. Additionally, I was able to make observations that required the entire large dataset, and I wasn't hesitant to handle it with Pandas. This didn't even occur to me while working with Excel at my job; I just wanted to stick to the trimmed dataset.

## Visual work for Power network

The main goal of this project was to learn how to use a new visualization tool, and this was also achieved, beyond expectations! I explored Rawgraphs but chose Flourish for creating the network graph. Initially, I struggled, but gradually I learned the program's logic and navigation. I am not satisfied with the network graph because it is not very readable. With a smaller dataset, the result would be better. I also created a hierarchical tree map, which also has room for improvement...

I am most satisfied with the SVG-D3 graph, which includes all board seats. I actually created it as Youyou's homework and realized later that I could include it in this project.

## HTML work for Power network
I used Soma's basic template and made some changes, using my first project's webpage as an example. I also used HTML code that I created as homework (SVG with D3).

## Webpage for Power network

https://armyniemela.github.io/powernetwork/
