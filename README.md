jQuery-Mobile-Toast
==========================

A toast notification is a message that pops up on the surface of the window. It only fills the amount of space required for the message and the user's current activity remains visible and interactive. The notification automatically fades in and out, and does not accept interaction events.

A toast is best for short text messages, such as "File saved," when you're fairly certain the user is paying attention to the screen.

It's a clone of the Android toast notification.


Suggested Use
-------------
The use of Toast is very simple.  Assuming a trigger of a usual button, i.e.:

	<a href='#' id='diag1' data-role='button'>Show toast notification</a>
	
Create a DIV with the content for the toast message, and set **data-role="toast"**:

	<div id="my_toast" data-role="toast">file saved.</div>
	
A typical Toast code block would look like:

	$('#diag1').live('vclick', function() {
		$('#my_toast').toast('show')
	});

