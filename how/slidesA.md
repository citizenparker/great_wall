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

<!SLIDE >

# Small Problems #

* Model growth
* Repetetive sinatra wiring

<!SLIDE>

# Medium #

	@@@ruby
	resource TimeOff, :base => '/timeoff' do
		default_actions :create, :retrieve, :query, :update, :delete

	end

<!SLIDE>
# Medium Problems #
* Different representations of models, more granular control
* More model information that remains serverside
* Performance / Scalability concerns

<!SLIDE>
# Large #
* Solutions may vary / TBD
* Presenters vs JSON views (read that Mojo? blog)

<!SLIDE subsection>
# The Client #

<!SLIDE>
# Many Ways to do this #
//TODO graphic of logos w/ jQuery, Knockout, SproutCore, Backbone, etc.
<!SLIDE>
# Our Ways to do this #
//Graphic of above with all but SproutCore and Backbone grayed out
<!SLIDE>
# Key Concepts #
Request / Response vs Run Loop
Bi directional communication

<!SLIDE >
# SproutCore #
 graphic on key architecture

<!SLIDE >

# Samples #
// Three-ish samples
// sample of Views
// DataSource
// Controller samples
// Models (derived attributes / binding)

<!SLIDE>

# Pros & Cons

<!SLIDE>

# Backbone #

graphic of architecture

<!SLIDE >

# Samples #
// Three-ish samples
// sample of Views
// Routes
// Collections
// Models (derived attributes / binding)

<!SLIDE>

# Pros & Cons #

<!SLIDE>

# SUMMATION? #
