# UFOs

## Project Overview

The purpose of this project was to create a webpage with a dynamic table that allows users to filter through the UFO sightings data based on multiple criteria. Initially, the table was only able to filter data based on the date. However, as a part of the challenge for this project, the table was updated so that it could be filtered based on one or more of the following filters: city, state, country, and UFO shape.

## Results

To better understand how the updated webpage works, below are few examples on the responsiveness of the table to our new filters:

Upon loading the webpage, the user will be presented with a non-filtered version of the table displaying all UFO sightings based on our "data.js" file:

![Unfiltered Table](https://github.com/josem279/UFOs/blob/master/Screenshots/Unfiltered%20table.PNG)

To filter the data in our table based on one input we would simply choose one input and type in the input box:

![FilteredTable1](https://github.com/josem279/UFOs/blob/master/Screenshots/FilteredTable1.PNG)

If our initial filter does not filter out enough rows from our table, we can apply another filter to further narrow our search. Again, this is done by entering valid text into the desired input box:

![FilteredTable2](https://github.com/josem279/UFOs/blob/master/Screenshots/FilteredTable2.PNG)

Assuming that we have entered sufficient info into our input boxes and have found the UFO sighting that we wanted, we can restart the process by either clearing the text in our input boxes or by clicking the link to the webpage at the top left. Both options result in an unfiltered data table:

![ResetTable](https://github.com/josem279/UFOs/blob/master/Screenshots/ResetTable.PNG)

## Summary

One potential drawback of this new design is that the webpage is that a misspelled word in any of the inputs results in an empty filtered table as it searches for the exact text that is entered into our inputs. Moreover, the search option is so exact that it does not search for partial entries in the inputs - for instance if we only type "c" in the state filter, it will not filter for all states startin with "c" it will instead create and empty table.

In order to improve upon the design of this webpage, I recommend making the following updates:

1. Updating our input filters so users can enter multiple values. This allows users to get a more refined search. For instance, instead of having to look for UFO sightings in two cities by carrying out two searches, users would be able to enter two city names in one search. This can be done by adding the "multiple" attribute in our "<input /> elements.

2. Setting a character limit on some fields so that it matches the data and ensures that the user correctly inputs data that matches what is in our table. For instance by setting a character limit on our input for State to 2 characters, users will know to use the abbreviated versions of states rather than the whole name. This update can easily be done by adding the "maxlength=" attribute in the "<input />" elements.
