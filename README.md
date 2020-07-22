# kn-admin-apps | version-1.1

## setup 
- clone project
- install mongo if not installed:   https://www.mongodb.com/try/download/community
- install npm and nodejs if not installed:   https://nodejs.org/en/download/
- run `npm install` in project directory to install dependencies

## usage
* make sure that mongo is running
* run `npm start` in project directory to run server

## development
* run `npm run dev` to run server and watch for changes
* run `npm run test` to run unit tests and watch for changes
***
***
> # changelog | 1.1
> 
> # global
> 
> ## features
> 
> - added "/store-select" route to login to a specific store
> 
> # shift-cards
> 
> ## features
> 
> - cards now display a simple "break" next to names instead of a proposed time to send them
> - cards now base their positions off the more specific position information rather than the schedule group
> - made topic data load based on the saved selected store
> - added a header in the settings panel to navigate to "/store-select"
> - made shift cards autodirect to "/store-select" if no store is selected
> - when shift cards directs to "/store-select" it is made to redirect back to shift cards after store is selected
> - shift cards will now index any new employees found upon card generation into the database (this is store specific)
> - added the concept of tabs in settings panel
> - added two functional tabs to switch between "employees" and "topics"
> - improved the look for the topics tab
> - in employees tab a list of any indexed names for a store is now displayed
> - the employees tab refreshes automatically after a user generates a shift card
> - added delete and edit button to each displayed employee
> - added deletion confirmation when delete is clicked
> - an edit view is shown when the edit button is pressed allowing for changing the alias and driver status for an employee
> - there is now an indicator by each employee showing their driver status
> - added search bar for filtering through employees
> - search bar does intelligent autoscrolling and animation effects to enhance search experience
> - search bar can filter employees by full name or alias
> - search bar can find anyone who is a driver by typing "drivers"
> - employee aliases and driver statuses saved to the database now appear on generated cards
> - all errors that could be created notify the user with a red banner at the bottom
> 
> ## removal
> 
> - all hard coded customization (driver list, alias list, break times)
> 
> ## bugs 
> 
> couldn't close settings panel when clicking inside the main header
> - topic text areas didn't always match the dimensions of their character counters
> - employees were being sorted in positions they weren't scheduled for
> - duplicate position lists were being created on the shift card output
> - success message displayed when updating topics is shown a second time whenever the user reloads the page
> - if a success banner is created after an error banner, the success banner is red instead of green
> - failed file upload in certain cases would throw 500 error instead of the expected 406 error
> ***
> ***
