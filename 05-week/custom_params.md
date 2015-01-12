#Lesson Index Card

###1. Custom Params in Rails

###2. Learning Objective(s)
* SWBAT use custom params to filter their index page.  
* SWBAT Understand that params is just a hash made out of strings that is passed from the browser to the server.  
* Know when to use custom params

###3. Essential Question(s)
* What does curstom params mean?
* What methods can you use for custom params?

###4. Talking Points/Road Map

###Recall what we did with our bean app to select by roasts, and students by grade

###Build a simple rails app and use custom params to just render a string on the next page

`rails new params_app -O -T`

#### Map root to HomeController#index
show a simple form on the homepage 

with a submit that points to HomeController#next
```
<%= form_tag({ controller: "home", action: "next" }) do %>
  My name is: <%= text_field_tag :name %>
  My favourite language is: <%= text_field_tag :favourite %>
  <%= submit_tag "Submit page" %>
<% end %>
```

### Have #next render the params as a nicely made up string
```
<%= form_tag({ controller: "home", action: "next" }) do %>
  My name is: <%= text_field_tag :name %>
  My favourite language is: <%= text_field_tag :favourite %>
  <%= submit_tag "Submit page" %>
<% end %>
```

