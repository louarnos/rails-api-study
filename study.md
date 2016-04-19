# Rails as an API Study

Use your favorite search engine and the provided readings to research and answer
the following questions (no prior knowledge is expected).

In your answers, be sure to cite any relevant sources you consulted in your
search. We ask you to write answers in your own words in order to see how you
process what you've read. Please do not answer with direct quotes from source
material. Instead, digest what you've read and repeat it in your own voice.

Please note:

-   Many of the readings will mention the "view" layer. We won't be covering the
    view layer in this program.
-   We'll use our [rails-api-template](/ga-wdi-boston/rails-api-template)
    repository as the basis for our rails applications.
    This template excludes the "view" layer.

## Required Readings

-   [Starting Ruby on Rails: What I Wish I Knew | BetterExplained](http://betterexplained.com/articles/starting-ruby-on-rails-what-i-wish-i-knew/)
-   [Intermediate Rails: Understanding Models, Views and Controllers | BetterExplained](http://betterexplained.com/articles/intermediate-rails-understanding-models-views-and-controllers/)
-   [Getting Started with Rails — Ruby on Rails Guides](http://guides.rubyonrails.org/getting_started.html)
-   [The Rails Command Line — Ruby on Rails Guides](http://guides.rubyonrails.org/command_line.html)
-   [Rails Routing from the Outside In — Ruby on Rails Guides](http://guides.rubyonrails.org/routing.html)
-   [Action Controller Overview — Ruby on Rails Guides](http://guides.rubyonrails.org/action_controller_overview.html)

## Define Model Responsiblities

In your own words, define what the responsibilities of the model layer are in
Rails.

```md
The model layer is what accesses and stores data in the database. It does this based on data passed to or requested from it.
```

## Define Controller Responsiblities

In your own words, define what the responsibilities of the controller layer are
in Rails.

```md
The controller acts the intermediary between things that are input or requested from the browser. It takes this information and then handles it accordingly so that what needs to be done with it can be done. This means either update the view, or pass data off to or request from models.
```

## Define Router Responsiblities

In your own words, define what the router does in Rails.

```md
A router takes a URL or request and directs it to the correct portion of the controller so that correct action can be taken. It can act dynamically depending on the request so that less hardcoding is necessary.
```

## The Request-Response Cycle in Rails

Starting with a client making a GET request to a particular URL, describe how
the parts of Rails interact to produce and send a response.

```md
The user makes the request from the browser. The router then decides what portion of the controller is needed to make this request, and passes the info the the controller. The controller then passes the request to the model that pulls the requested info from the database, and the request is then passed back through this chain to the controller where the info is then distributed back to the user in some way. 
```
