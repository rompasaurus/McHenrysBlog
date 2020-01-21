---
layout: post
title:  "Thought Input Page"
date:   2020-01-21 
categories: [Overview,Planning,Goals,Homepage]
---
### Thought Input Page:
This is the heart of the web site and the idead behind the site. This willhighly interactive page that will react to specific characters input on the page. Forms and drops downs should not exist on this page its should flow interactively after the the enter button is hit.Topics or subtopis should be trigger upon typing a colon and enter on the keyboard.

### Worflow:	
User starts by typing their first topic followed by a colon
	Topic: >
Upon  hittin enter if the topic has not been mentioned before user is prompted to outline a quite detail behind the topic subject and its purpose in journalling.
	Please input topic outline and details: general outline of what will be expanded on within this topic context 
	User can ype in the details here or hit enter to skip to the content of the post and topic description can be entered at a later date
Content Body input
	Cursor is tabbed over and the Heart of the topic details typed here.
Enter Once > sub topic :
	user can establish a subtopic here again will be prompted to outline a descripttion that can be entered past.
Enter Twice:
	Ends current topic discourse and brings user back one tab to the left indicating that the main or subtopic topic discourse has ended.

	
### Style:
Decided to add some coler to the site Gray and lots of it. This site is gonna be straight up 90's but with interactivity. A throw back.Spent some time figuring out the nav bar up to to stay at the top even when scrolling down.


### Example Snippet:
[Template Output](/assets/CaptureInputPage.PNG)

### Code:
	<!DOCTYPE html><html lang="en-US">
<style>
body {
  margin: 0;
  font-size: 20px;
  font-family: Arial, Helvetica, sans-serif;
}

#Navigation_Bar{
	overflow: hidden;
	background-color: grey;
	width:100%;
}
.Site_Logo{
	text-align: center;
	margin-right:200px;
}

#Navigation_Bar a {
  float: left;
  display: block;
  color: black;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
  font-size: 17px;
}

.Right_Sidebar {
  width: 200px;
  position: fixed;
  z-index: 1;
  top: 0;
  right: 0;
  background-color: darkgray;
  padding-top: 140px;
  height:100%;
}
.Right_Sidebar a {
  padding: 60px 8px 10px 16px;
  text-decoration: none;
  font-size: 16px;
  color: black;
  display: block;
}

.Content {
  padding-top: 20px;
  padding 16px;
  margin-left: 16px; 
  margin-right: 210px;/* Same as the width of the right and left sidebar */
}
#Navigation_Bar a:hover {
  background-color: white;
  color: green;
}

#Navigation_Bar a.active {
  background-color: green;
  color: white;
}


/* The sticky class is added to the navbar with JS when it reaches its scroll position */
.sticky {
  position: fixed;
  top: 0;
  width: 100%;
}

/* Add some top padding to the page content to prevent sudden quick movement (as the navigation bar gets a new position at the top of the page (position:fixed and top:0) */
.sticky + .content {
  padding-top: 60px;
}
	</style>
	<html>
		<head></head>		
		<title class="site_name"> The Thought Encyclopedia </title>
		<h1 class="Site_Logo">The Thought Encyclopedia</h1>
	
	<div id="Navigation_Bar">
		<a href="/" class="item">Home</a>
		<a href="/ruminations">Ruminate</a>                 
		<a href="/login">Username//Login</a>
		<a href="/about">About</a>                 
	</div>
	
	<div class="Content">
		<body>
			<div class="Ruminations">
				<h2 class="home page title">Ruminations:</h2>
				<div class="thought snippet">
					<h3>Thought topic title:</h3>
					<p class="topic content">
						Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum
					</p>
				</div>
				<div class="thought_snippet">
					<h3>Thought topic title number 2:</h3>
					<p class="topic_content">
						Praesent tellus massa, efficitur vitae enim quis, imperdiet maximus enim. Curabitur consequat nibh nunc, at blandit libero volutpat posuere. Nam at ex rhoncus, fermentum turpis sed, tincidunt neque. Phasellus diam dolor, tristique efficitur malesuada eget, convallis vel metus. Curabitur ullamcorper erat at dui dignissim consectetur. Praesent hendrerit libero a egestas feugiat. Donec convallis vestibulum urna. Ut sed diam non justo euismod dignissim. Vivamus in turpis a purus maximus faucibus quis a justo. Nulla sed orci eget velit porta luctus a ac purus. Duis porta at lacus viverra varius. In cursus rutrum lectus, vitae dignissim enim laoreet at. Suspendisse vitae enim gravida, efficitur tortor ac, bibendum nunc. Maecenas fringilla tempus metus, quis tempus felis. Etiam sed est justo.
					</p>
				</div>
				<div class="thought_snippet">
					<h3>Thought topic title number 3:</h3>
					<p class="topic_content">
						Integer vitae interdum leo. Aliquam fermentum elit ut justo luctus pharetra. Nulla erat lectus, auctor eget interdum ac, posuere et ex. Phasellus rutrum dignissim magna, in sagittis turpis ultricies vel. In eget mi ullamcorper, commodo odio ut, auctor ex. Donec congue, risus eu tempor dignissim, felis urna consectetur libero, id sodales nisi sapien non erat. Suspendisse sed est felis. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Ut laoreet laoreet lectus ut condimentum. Vivamus mollis molestie ipsum quis dignissim. Etiam fringilla ultricies tincidunt. Duis a laoreet nisl. Vivamus nec mauris sed ligula sodales tincidunt.
					</p>
				</div>
				<div class="thought_snippet">
					<h3>Thought topic title number 4:</h3>
					<p class="topic_content">
						Integer vitae interdum leo. Aliquam fermentum elit ut justo luctus pharetra. Nulla erat lectus, auctor eget interdum ac, posuere et ex. Phasellus rutrum dignissim magna, in sagittis turpis ultricies vel. In eget mi ullamcorper, commodo odio ut, auctor ex. Donec congue, risus eu tempor dignissim, felis urna consectetur libero, id sodales nisi sapien non erat. Suspendisse sed est felis. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Ut laoreet laoreet lectus ut condimentum. Vivamus mollis molestie ipsum quis dignissim. Etiam fringilla ultricies tincidunt. Duis a laoreet nisl. Vivamus nec mauris sed ligula sodales tincidunt.
					</p>
				</div>
				<div class="thought_snippet">
					<h3>Thought topic title number 5:</h3>
					<p class="topic_content">
						Integer vitae interdum leo. Aliquam fermentum elit ut justo luctus pharetra. Nulla erat lectus, auctor eget interdum ac, posuere et ex. Phasellus rutrum dignissim magna, in sagittis turpis ultricies vel. In eget mi ullamcorper, commodo odio ut, auctor ex. Donec congue, risus eu tempor dignissim, felis urna consectetur libero, id sodales nisi sapien non erat. Suspendisse sed est felis. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Ut laoreet laoreet lectus ut condimentum. Vivamus mollis molestie ipsum quis dignissim. Etiam fringilla ultricies tincidunt. Duis a laoreet nisl. Vivamus nec mauris sed ligula sodales tincidunt.
					</p>
				</div>
				<div class="thought_snippet">
					<h3>Thought topic title number 6:</h3>
					<p class="topic_content">
						Integer vitae interdum leo. Aliquam fermentum elit ut justo luctus pharetra. Nulla erat lectus, auctor eget interdum ac, posuere et ex. Phasellus rutrum dignissim magna, in sagittis turpis ultricies vel. In eget mi ullamcorper, commodo odio ut, auctor ex. Donec congue, risus eu tempor dignissim, felis urna consectetur libero, id sodales nisi sapien non erat. Suspendisse sed est felis. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Ut laoreet laoreet lectus ut condimentum. Vivamus mollis molestie ipsum quis dignissim. Etiam fringilla ultricies tincidunt. Duis a laoreet nisl. Vivamus nec mauris sed ligula sodales tincidunt.
					</p>
				</div>
			</div>
		<footer>
			<center>
			    <div class="footer">
			        <p>This website was created by Michael McHenry</p>
			        <div class="contact_links">
			            <a href="https://github.com/rompasaurus">Github Page</a>
			            <a href="https://www.linkedin.com/in/michael-mchenry-72416994">Linkedin Page</a>
			            <a class="twitter"href="http://twitter.com/share">Share On Twitter </a>
			        </div>
			    </div>	
			</center>
		</footer>
	</div>
	<div class="Right_Sidebar">
		<a href="topiclink">Topic Category 1</a>
		<a href="topiclink">Topic Category 2</a>
		<a href="topiclink">Topic Category 3</a>
		<a href="topiclink">Topic Category 4</a>
		<a href="topiclink">Topic Category 5</a>
		<a href="topiclink">Topic Category 6</a>
		<a href="topiclink">Topic Category 7</a>
		<a href="topiclink">Topic Category 8</a>
	</div>
	<script>
	window.onscroll = function() {myFunction()};

	// Get the navbar
	var Navigation_Bar = document.getElementByID("Navigation_Bar");

	// Get the offset position of the navbar
	var sticky = Navigation_Bar.offsetTop;

	// Add the sticky class to the navbar when you reach its scroll position. Remove "sticky" when you leave the scroll position
	function myFunction() {
	  if (window.pageYOffset >= sticky) {
	    Navigation_Bar.classList.add("sticky")
	  } else {
	    Navigation_Bar.classList.remove("sticky");
	  }
	}
	</script>
	</body>
	</html>
