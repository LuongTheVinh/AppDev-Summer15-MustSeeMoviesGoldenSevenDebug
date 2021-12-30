# Resource Practice

This application has 4 database-backed web CRUD resources: directors, movies, roles, and actors.

As usual, each resource has 7 "golden" actions that allow users to interact with it:

### CREATE
 - new_form
 - create_row

### READ
 - index
 - show

### UPDATE
 - edit_form
 - update_row

### DELETE
 - destroy

There are bugs in most of the 28 actions required to CRUD our 4 resources. Your job is to debug them all until you can create, read, update, and delete each of directors, movies, roles, and actors without running into any issues.

Here is a fully functional version of the app, for your reference.

https://resource-practice.herokuapp.com/

Make yours work like it. Your local app is using a dark Bootswatch, and the reference app is using a light Bootswatch; don't get confused between the tabs as you try to check your work.

## Setup

 1. Fork and then clone.
 1. `cd` to its location.
 1. `bundle install`
 1. `rake db:migrate` (To create the four tables on your machine; I have already written the instructions to do so.)
 1. `rake db:seed` (to pre-populate your tables with some data, so we can get straight to work. This step may take a while on Windows machines. You can open a new Command Line window to continue working while it runs.)
 1. `rails server`

Navigate to

http://localhost:3000

You should see a list of movies. The `Movies#index` action is functional, and I have set it to be the root URL.

From here, click through the app and debug. Try adding a new movie, updating a movie, looking at the details of a movie, and deleting a movie.

Sometimes you will get an error message; sometimes there won't be an error message, but the action just won't do its job. Use the server log to help figure out what's going on.

After Movies, work on Directors, then Actors, then Roles.
