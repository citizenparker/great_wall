<!SLIDE bullets incremental>

# Problems #
* Different consumers
* Richer experiences
* Expansive codebases

<!SLIDE >

# Consumers #

![tbd](../images/tbd.gif)

<!SLIDE>

# Richer Experiences #

// saner way to create rich experiences
// embracing JS rather than distrusting it

<!SLIDE subsection>

# Key to "Cheap" Scale #


<!SLIDE>
# Scale of Complexity #
// isolating and structuring complexity inherently easier when everything is already an API or service
// transitions between architectures are cheaper

<!SLIDE>
# Scale of Performance #
// offloading UI code to clients
.notes
  Success of this requires a strict mentality in isolating data and providing keys to find further data as opposed to megablobs
  See also: Facebook Graph API (code example?)

<!SLIDE>
# Scale of Organization #

// smaller mental models - faster ramp-up time
// separation of organizational concerns / easier team splits

<!SLIDE>

# Additional Considerations #

// Think about how not only client consumes API, but how API endpoints interact w/ one another

<!SLIDE>
// Remaining decoupled while still useful

<!SLIDE>
// Do we need MVC on "both sides" of the wall?

<!SLIDE>
// stateless-ness of this model. State of the client-interactions are managed on the client, and the server manages the persistence/state of the business domain