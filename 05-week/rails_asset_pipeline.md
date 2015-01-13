#Lesson Index Card

###1. Lesson Topic/Title

###2. Learning Objective(s)
* Students will be able to have a basic understanding of the rails asset pipeline
* Know how to limit asset pipeline behaviors
* Add and remove files from the application manifests
* Know what precompiled assets means


###3. Essential Question(s)
What is fingerprinting?
WHat does the asset pipeline do?

###4. Talking Points/Road Map
* Add in a custom css sheet into the asset pipeline.

* Go over what the `style_sheet_link_tag` and the `javascript_include_tag` do

* Then add in another conflicting stylesheet and show how we can use controller specific style rules in the controller.scss files so a controller uses different stylesheets. Use params[:controller] in application.html.erb

* Have a sample app with two models, `SchoolBus` and `Firetruck` have the students figure out how to make all the firetruck pages have firetruck red styling and the schoolbus pages have all yellow styling.

* Show that application.html.erb is just another embedded ruby file, we can have `if...else` statements in there just like anywhere else.

* Practice precompiling assets locally and give examples of how this could be needed in the real world (heroku).
