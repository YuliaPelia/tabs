# tabs
tabs
tabsSelector - tabs on which we will click
tabsContentSelector - a div that stores the content corresponding to our tabs
tabsParentSelector - stores all tabs in itself
activeClass - activity class that will switch to the tabs in which the event occurred
1. I get all the necessary elements from the page
2. I am creating a function that will hide all tabs that are not called
* I work with the activity class (active), when we hide all the tabs from visibility, then I will take the activity class from all the tabs that are there
* going through all the tabs, I will delete the class (active) in each tab
3. I create a function that will show us a tab
* 0 means that we transfer the first slide at the beginning
* I use css styles to display the tab we need
4. Define event delegation and assign a click event handler
* allocate e.target to a separate variable so as not to write it every time
* I will use the contains tool to determine whether the tab was clicked
* when clicking on a certain element, it is necessary to allocate its number in the list of all tabs 
and call the function that will show the required tab (showTabContent) based on this number, 
this is done by the usual sorting
