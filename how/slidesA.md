<!SLIDE subsection>

# Building the API #

<!SLIDE>

# Three Phases of API Architecture #

<!SLIDE>

# Small #

	@@@ ruby
	require 'sinatra'

	get '/todos' do
  		Todo.all.to_json
	end

<!SLIDE bullets incremental>

# Small Problems #

* Model growth
* Repetitive Sinatra wiring

<!SLIDE>

# Medium #

	@@@ruby
	resource TimeOff, :base => '/timeoff' do
		default_actions :create, :retrieve, 
			:query, :update, :delete

	end

<!SLIDE bullets incremental>
# Medium Problems #
* Different representations of the same model
* Growing model information that remains server-side
* Performance / scalability concerns

<!SLIDE bullets incremental>
# Large #
* Presenters
* JSON views ([RABL](https://github.com/nesquena/rabl), for instance)

<!SLIDE subsection>
# The Client #

<!SLIDE center>
# Many Ways to do this #

![tbd](../images/all_frameworks.jpg)

## ...

<!SLIDE center>
# Our Ways to do this #
![tbd](../images/our_frameworks.jpg)

## ...

<!SLIDE>
# Clientside MVC Is Different! #

<!SLIDE center>
![server](../images/server_mvc.png)

## Server-side MVC

<!SLIDE center>
![server](../images/client_mvc.png)

## Client-side MVC

<!SLIDE center>
# SproutCore in Three Acts#
![sc](../images/sproutcore.png)

<!SLIDE >
# Samples #
// Three-ish samples
// sample of Views
// DataSource
// Controller samples
// Models (derived attributes / binding)

<!SLIDE>

# Pros & Cons

<!SLIDE center>

# Backbone in Three Acts #

![sc](../images/backbone.png)

<!SLIDE >

# Samples #
// Three-ish samples
// sample of Views
// Routes
// Collections
// Models (derived attributes / binding)

<!SLIDE>

# Pros & Cons #