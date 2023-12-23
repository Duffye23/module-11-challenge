# module-11-challenge
The Challenge was to use both Splinter and Beautfiul to scrape the given NASA webpages and extract relevant information. In the first half of the challenge, we were tasked to pull article titles and their accompanying text previews. </br>
Imported Libraries used in part 1:</br>
![image](https://github.com/Duffye23/module-11-challenge/assets/58863493/641f0b31-fe41-4394-ae8f-f1ba7180a065)</br>

It should be noted that if your version of Google Chrome is newer than version 118, you should use the following steps in the command line:</br>
![image](https://github.com/Duffye23/module-11-challenge/assets/58863493/68eb2e9b-160c-4097-a26a-6f99a7c50ab5)</br>
Also note that this should be run on each notebook everytime it is opened. I thought this would not be necessary but I discovered this to be required, at least for my machine.</br>

I cannot stress the importance of running these commands line by line in the command line instead of in the notebook; the notebook had the first line running upwards of 12 minutes with no progress, whereas the command finished each line near instantaneously.</br>

With the BeautifulSoup object created, we were able to pull the text of the listed tags and then extract the titles and preview texts. From there I placed it into a dictionary and then a list via a loop so that we can view every title and preview text as asked.

The for loop: </br>
![image](https://github.com/Duffye23/module-11-challenge/assets/58863493/e380da83-23cf-43ac-a7d9-400d79c1936f)</br>

A section of the finished list: </br>
![image](https://github.com/Duffye23/module-11-challenge/assets/58863493/093a00f7-82c8-4c56-97a9-3ee4f38dfa3e)</br>

For Part 2, it was much of the same thing: We were tasked with pulling a table out from a webpage this time. This was expanded upon afterwards with having to perform analysis on the extracted table.
We had to change the data type of the table into int and float so that they could be manipulated further.</br>
Scraping the webpage and turning it into a dataframe for analysis:</br>
![image](https://github.com/Duffye23/module-11-challenge/assets/58863493/46d0b7d4-1469-4267-be4b-2511d01fb6c5)</br>
![image](https://github.com/Duffye23/module-11-challenge/assets/58863493/77315d16-92ee-4b51-8b3c-1898e9d3aad2)</br>

Changing the datatypes of the columns:</br>
![image](https://github.com/Duffye23/module-11-challenge/assets/58863493/db586ab7-77bb-4d91-90d8-fe622093dbde)</br>

Finally, using gorup_by(), we can manipulate the data and create the charts requested.</br>
![image](https://github.com/Duffye23/module-11-challenge/assets/58863493/84813641-bd37-4d95-817c-4e2b72eaeac8)</br>
![image](https://github.com/Duffye23/module-11-challenge/assets/58863493/f92d3f9e-0ba3-41d5-af5b-2c117adfd9c9)</br>

I had to switch to using matplotlib as the plotting source for the final question, shown below:</br>
![image](https://github.com/Duffye23/module-11-challenge/assets/58863493/103469b1-4f43-4f3d-ae1e-fbd363f4c1c9)</br>

We can tell from rough distance between the peak temparatures that the total earth days that a year on Mars comes out to be roughly 675. A quick search reveals that the actual amount of days to be 687 Earth days to a Martian year.

Sources used:</br>
Carleton Bootcamp Modules 11 and 12 learning activites</br>
AskBCS Help Channel for the help in fixing the Chrome version issue.</br>
Changing dtypes for an entire df: https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.astype.html</br>
Changing a single column's dtype: https://stackoverflow.com/questions/17134716/convert-dataframe-column-type-from-string-to-datetime</br>
Setting labels for x and y axes: https://stackoverflow.com/questions/21487329/add-x-and-y-labels-to-a-pandas-plot</br>






