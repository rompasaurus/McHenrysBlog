---
layout: post
title:  "Home Page Planning"
date:   2020-01-18 
categories: [Overview,Planning,Goals,Homepage]
---
### Home Page Planning
This post is meant to outline the basic structure and template that I would like to use to act as the landing page to the thought encylopedia. 
There is going to be 2 tailored home page landings 1 trigger when the user first arrives at the site and is not logged in and the other will be for the user once he logs in

### Un-Authenticated landing page:

#### User Story:

The user will begin their journy to site and be offered a landing page that showcases the most popular and trendign public facing thought entries from all members of the site. The body of the site will be the post topic title and first 300-500 characters of the content. on the left side of the content will be a list of pupular topic catgories the user can select to view post related to some of the most popular content types in use currently.

#### Theme:

Going to stay basic for the time being simple divs and html tags with verbose class names. Key is to be basic but allow for easy styling when it comes a point to intoduce a bit of flair and graphics to the site.
Simple header and footer Vertically arrange header links

#### Header Links:
	Home , About , Todays Ruminations, Usenamae//Login, Most Wrote about topic 1,topic 2, topic 3.

#### Footer:
	Contact, Creator, year mark, github page, 

#### HTML and SUBLIME text notes
Delete the entire tag opening and closing :

Install the emmet plugin and use the command ctrl+shift+; while inside the tage and it will be auto deleted

Adding a sidebar:
	<div class="Popular_Topic_Sidebar">
			<a href="topiclink">Topic 1</a>
			<a href="topiclink">Topic 2</a>
			<a href="topiclink">Topic 3</a>
			<a href="topiclink">Topic 4</a>
			<a href="topiclink">Topic 5</a>
			<a href="topiclink">Topic 6</a>
			<a href="topiclink">Topic 7</a>
			<a href="topiclink">Topic 8</a>
	</div>
A sidebar needs a bit of styling and orientation oof the other elemnts around it befor it can be view properly
css:
	Popular_Topic_Sidebar {
	  height: 100%;
	  width: 160px;
	  position: fixed;
	  z-index: 1;
	  top: 0;
	  left: 0;
	  background-color: white;
	  padding-top: 16px;
	}

	.Popular_Topic_Sidebar a {
	  padding: 6px 8px 10px 16px;
	  text-decoration: none;
	  font-size: 20px;
	  color: black;
	  display: block;
	}

	.Main {
	  margin-left: 160px; /* Same as the width of the sidenav */
	  padding: 0px 10px;
	}

Full Homepage code and preview:

	<!DOCTYPE html><html lang="en-US">
	<style>
	body {font-family: "Lato", sans-serif;}

	.Popular_Topic_Sidebar {
	  height: 100%;
	  width: 160px;
	  position: fixed;
	  z-index: 1;
	  top: 0;
	  left: 0;
	  background-color: white;
	  padding-top: 16px;
	}

	.Popular_Topic_Sidebar a {
	  padding: 6px 8px 10px 16px;
	  text-decoration: none;
	  font-size: 20px;
	  color: black;
	  display: block;
	}

	.Main {
	  margin-left: 160px; /* Same as the width of the sidenav */
	  padding: 0px 10px;
	}

	@media screen and (max-height: 450px) {
	  .sidebar {padding-top: 15px;}
	  .sidebar a {font-size: 18px;}
	}
	</style>
	<html>
		<title class="site_name"> The Thought Encyclopedia </title>
		<div class="Main">
			<head>
				<h1 class="Site_Logo">The Thought Encyclopedia</h1>
				<div class="Navigation_Bar">
					<a href="/" class="item">Home</a>
		            <a href="/ruminations" class="item">Todays Ruminations</a>                 
		            <a href="/login" class="item">Username//Login</a>
		            <a href="/about" class="item">About</a>                 
				</div>
			</head>

			<body>
					<div class="thoughts_of_the_day">
						<h2 class="home page title">Thoughts Of The Day</h2>
						<div class="thought snippet">
							<h3>Thought topic title</h3>
							<p class="topic content">
								Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum
							</p>
							<p class="user link"><a href="link to user">Username</a></p>
							<p class="snippet date">01/18/2020</p>
							<p class="snippet meta">
								<a href="Upvote">Upvote</a>
								<a href="Downvote">Downvote</a>
								<a href="Favorite">Favorite</a>
								<a href="Share">Share</a>
							</p>
						</div>
						<div class="thought_snippet">
							<h3>Thought topic title number 2</h3>
							<p class="topic_content">
								Praesent tellus massa, efficitur vitae enim quis, imperdiet maximus enim. Curabitur consequat nibh nunc, at blandit libero volutpat posuere. Nam at ex rhoncus, fermentum turpis sed, tincidunt neque. Phasellus diam dolor, tristique efficitur malesuada eget, convallis vel metus. Curabitur ullamcorper erat at dui dignissim consectetur. Praesent hendrerit libero a egestas feugiat. Donec convallis vestibulum urna. Ut sed diam non justo euismod dignissim. Vivamus in turpis a purus maximus faucibus quis a justo. Nulla sed orci eget velit porta luctus a ac purus. Duis porta at lacus viverra varius. In cursus rutrum lectus, vitae dignissim enim laoreet at. Suspendisse vitae enim gravida, efficitur tortor ac, bibendum nunc. Maecenas fringilla tempus metus, quis tempus felis. Etiam sed est justo.
							</p>
							<p class="user link"><a href="link to user">Username</a></p>
							<p class="snippet date">01/18/2020</p>
							<p class="snippet meta">
								<a href="Upvote">Upvote</a>
								<a href="Downvote">Downvote</a>
								<a href="Favorite">Favorite</a>
								<a href="Share">Share</a>
							</p>
						</div>
						<div class="thought_snippet">
							<h3>Thought topic title number 3</h3>
							<p class="topic_content">
								Integer vitae interdum leo. Aliquam fermentum elit ut justo luctus pharetra. Nulla erat lectus, auctor eget interdum ac, posuere et ex. Phasellus rutrum dignissim magna, in sagittis turpis ultricies vel. In eget mi ullamcorper, commodo odio ut, auctor ex. Donec congue, risus eu tempor dignissim, felis urna consectetur libero, id sodales nisi sapien non erat. Suspendisse sed est felis. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Ut laoreet laoreet lectus ut condimentum. Vivamus mollis molestie ipsum quis dignissim. Etiam fringilla ultricies tincidunt. Duis a laoreet nisl. Vivamus nec mauris sed ligula sodales tincidunt.
							</p>
							<p class="user_link"><a href="link to user">Username</a></p>
							<p class="snippet_date">01/11/2020</p>
							<p class="snippet_meta">
								<a href="Upvote">Upvote</a>
								<a href="Downvote">Downvote</a>
								<a href="Favorite">Favorite</a>
								<a href="Share">Share</a>
							</p>
						</div>
					</div>
			</body>
			<footer>
			    <div class="footer">
			        <p>This website was created by Michael McHenry</p>
			        <div class="contact_links">
			            <a href="https://github.com/rompasaurus">Github Page</a>
			            <a href="https://www.linkedin.com/in/michael-mchenry-72416994">Linkedin Page</a>
			            <a class="twitter"href="http://twitter.com/share">Share On Twitter </a>
			        </div>
			    </div>
			</footer>
		</div>
	<div class="Popular_Topic_Sidebar">
			<a href="topiclink">Topic 1</a>
			<a href="topiclink">Topic 2</a>
			<a href="topiclink">Topic 3</a>
			<a href="topiclink">Topic 4</a>
			<a href="topiclink">Topic 5</a>
			<a href="topiclink">Topic 6</a>
			<a href="topiclink">Topic 7</a>
			<a href="topiclink">Topic 8</a>
	</div>
	</html>