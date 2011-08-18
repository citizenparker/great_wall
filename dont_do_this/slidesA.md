<!SLIDE subsection>

# Five Bad Habits to Check at the Door #

<!SLIDE>

## #1. Monolithic mega-views

<br><br>

	@@@ html
	<!-- in your view... -->
	- if user.administrator?
		<!-- a bunch of cool admin-only stuff -->

<!SLIDE>

## #2. Endless relationship traversals

<br><br> 

	@@@ html
	<!-- in your view... -->
	Primary Customer:
	= company.invoices.first.buyer.first_name

<!SLIDE>

## #3. Flash abuse

<br><br>

	@@@ ruby
	flash[:show_fruit_baskets] = true if
		flash[:just_clicked_on_a_fruit]
		
<!SLIDE>

## #4. Lazy Javascript

<br><br>

	@@@ javascript
	$(function(){
		//just wrapping this in a onReady
		//protecter cause that's what you do
		...
	});
	
<!SLIDE>

## #5. Careless Deployments

.notes deployment synchroniziation (open browsers and how they react?) - THESE PAGES AREN’T RELOADING THE JS ON-CLICK BRO.	