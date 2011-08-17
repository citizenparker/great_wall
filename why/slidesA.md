<!SLIDE bullets>

# Problems #
* <span class="highlight">Different consumers</span>

<!SLIDE center>

![tbd](../images/consumers.png)

<!SLIDE bullets>

# Problems #
* Different consumers
* <span class="highlight">Richer experiences</span>

<!SLIDE bullets incremental>

# Richer Experiences #

* More desktop like user experience through enhanced client side code
* Entrust JavaScript rather than distrusting it
* What is the sane way to architect a system that accomplishes this?

<!SLIDE bullets>

# Problems #
* Different consumers
* Richer experiences
* <span class="highlight">Expansive codebases</span>

<!SLIDE bullets>

# Expansive codebases #

* How does this architecture make our lives easier as we scale?

<!SLIDE subsection>

# Key to "Cheap" Scale #

<!SLIDE bullets>
# Scale of Complexity #

* Structuring complexity more intuitive when everything is already an API or service
* Transitions between architectures are cheaper when you're oriented towards separation of concerns

<!SLIDE bullets>
# Scale of Complexity #

* Isolate parts of your app that are likely to change
* UI and user facing components are more volatile

<!SLIDE bullets>
# Scale of Performance #

* Off-load UI rendering to clients

<!SLIDE center>

![tbd](../images/scale1.png)

<!SLIDE bullets>
# Scale of Performance

* If you're disciplined in keeping your API silos isoalted, you can scale horizontally with ease

<!SLIDE center>

![tbd](../images/scale2.png)

<!SLIDE bullets center>
# Scale of Organization #

![tbd](../images/people.png)

* Leaner slices and mental models = faster ramp-up time
* Separation of organizational concerns = easier team splits

<!SLIDE bullets>

# Additional Considerations #

* Client consumes API, but API endpoints may also need to interact
* Psychology of the architecture is different as a developer

<!SLIDE bullets>
# Additional Considerations #
* Do we need MVC on "both sides" of the wall?

<!SLIDE bullets>
# Additional Considerations #
* State or lack thereof
* State of the client-interactions are managed on the client
* Server manages the persistence/state of the business domain
