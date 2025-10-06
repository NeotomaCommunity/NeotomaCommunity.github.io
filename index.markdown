---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---

<style>
#main {
  margin-left: 10%;
  margin-right: 10%;
}
  
</style>

<head>
  <title>Neotoma Community Stories</title>
</head>
<div id="main">
<div style="display:grid;grid-template-rows: 1fr 1fr; margin: 3%; margin-bottom: 0%;">
<div style="position: relative; border: 1px solid var(--neotoma-brown-450); background: linear-gradient(135deg, var(--neotoma-gray-150) 0%, var(--neotoma-brown-0) 100%); width: 136%; padding-top: 20px; display:grid; grid-template-columns: 1fr 5fr; align-items:center; justify-items: center; justify-self:center;">
  <img style="width:100px;padding-bottom:15px;" src="/images/many_rats.png"/>
<h1>{{ site.title }}</h1>
</div>
<div style="text-align: center; margin-left: 5%; margin-right: 5%;">
<p style="border-bottom: 1px solid var(--neotoma-brown-250);"> This website is a repository of stories contributed by members of Neotoma's community, organized by Neotoma's <a href="https://www.neotomadb.org/outreach" target="_blank"> Outreach and Community Engagement</a> team.</p>
</div>
</div>

<div style="display: grid; grid-template-rows: 1fr 10fr;">
  <h2 style="margin-top: 0px; padding-top: 0px;">Contributed Posts</h2>
<ul>
{% for post in site.posts %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <span> - {{ post.date | date: "%B %-d, %Y" }}</span>
  </li>
{% endfor %}


</ul>
</div>
</div>


<div class="offcanvas offcanvas-start" id="pagesModal" tabindex="-1" role="dialog" aria-modal="true" aria-labelledby="offcanvas-heading" aria-hidden="true">
	
<div class="offcanvas-content" role="document">
     
<button type="button" class="close" data-bs-dismiss="offcanvas" aria-label="Close">
<span class="visually-hidden">Close Navigation Menu</span>
<img src="/assets/images/modal-close-icon.svg" class="icon-close" alt=""><span class="visually-hidden">Close Navigation Menu</span>          
</button>
    
<div class="panel-nav">
<nav class="navbar">
<div class="container d-block">
<div class="row mx-0 d-flex justify-content-center">

<div class="col-12 col-md-8">

<p id="offcanvas-heading" class="visually-hidden">Site Navigation Menu</p>

<ul class="navbar-nav">

<li><a class="nav-link" href="/">Home</a></li>

<!-- About -->
 
<li class="nav-item dropdown">
<a class="nav-link dropdown-toggle" href="#" id="offcanvasNavbarAbout" role="button" data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">Neotoma <img src="/assets/images/carat.svg" alt=""></a>
	
<div class="dropdown-menu" aria-labelledby="offcanvasNavbarAbout">
<a class="dropdown-item" href="https://www.neotomadb.org/about">Neotoma Overview</a>
				 	
<a class="dropdown-item" href="https://www.neotomadb.org/about/governance">Governance</a>
<a class="dropdown-item" href="https://www.neotomadb.org/about/funders-partners">Funders &amp; Partners</a>
<a class="dropdown-item" href="https://www.neotomadb.org/about/join-the-neotoma-community">Join the Neotoma Community</a>
</div>
</li>

<!-- Data -->
  
<li class="nav-item dropdown">
<a class="nav-link dropdown-toggle" href="#" id="offcanvasNavbarData" role="button" data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">Data <img src="/assets/images/carat.svg" alt=""></a>
	
<div class="dropdown-menu" aria-labelledby="offcanvasNavbarData"> 
<a class="dropdown-item" href="https://www.neotomadb.org/data">Data Overview</a>
				 	
<a class="dropdown-item" href="https://www.neotomadb.org/data/constituent-databases">Constituent Databases</a>
<a class="dropdown-item" href="https://www.neotomadb.org/data/dataset-search">Find Data</a>
<a class="dropdown-item" href="https://www.neotomadb.org/data/contribute-data">Contribute Data</a>
<a class="dropdown-item" href="https://www.neotomadb.org/data/db-snapshots">DB Snapshots</a>
<a class="dropdown-item" href="https://www.neotomadb.org/data/data-use-and-embargo-policy">Data Use and Embargo Policy</a>
</div>
</li>
       
<!-- Apps -->
     	   
<li class="nav-item dropdown">
<a class="nav-link dropdown-toggle" href="#" id="offcanvasNavbarApps" role="button" data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">Apps  <img src="/assets/images/carat.svg" alt=""></a>
	
<div class="dropdown-menu" aria-labelledby="offcanvasNavbarApps">  
<a class="dropdown-item" href="https://www.neotomadb.org/apps">Apps Overview</a>
				 	
<a class="dropdown-item dropdown-item-external" href="https://www.neotomadb.org/apps/explorer">Explorer</a>
<a class="dropdown-item dropdown-item-external" href="https://www.neotomadb.org/apps/api">API</a>
<a class="dropdown-item" href="https://www.neotomadb.org/apps/tilia">Tilia</a>
<a class="dropdown-item dropdown-item-external" href="https://www.neotomadb.org/apps/neotoma-r">R package</a>
<a class="dropdown-item" href="https://www.neotomadb.org/apps/third-party-apps">Third-Party Apps</a>
</div>
</li>

<!-- Education -->
  
<li class="nav-item dropdown">
<a class="nav-link dropdown-toggle" href="#" id="offcanvasNavbarEducation" role="button" data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">Outreach  <img src="/assets/images/carat.svg" alt=""></a>
	
<div class="dropdown-menu" aria-labelledby="offcanvasNavbarEducation">
<a class="dropdown-item" href="https://www.neotomadb.org/outreach">Outreach Overview</a>
				 	
<a class="dropdown-item" href="https://www.neotomadb.org/outreach/lapd-ciclo-de-charlas-2025">Ongoing and Past Webinar Series</a>
<a class="dropdown-item" href="https://www.neotomadb.org/outreach/outreach-and-community-engagement-team">Outreach and Community Engagement Team</a>
<a class="dropdown-item" href="https://www.neotomadb.org/outreach/outreach-and-community-engagement-resources-inventory">Outreach and Community Engagement Resources Inventory</a>
<a class="dropdown-item" href="https://www.neotomadb.org/outreach/core-tutorials">Recommended Data Tutorials</a>
</div>
</li>

<!-- News -->
<li>
<a class="nav-link"  href="/news-events/" >News &amp; Events</a>
</li>

<!-- Resources -->
   
<li class="nav-item dropdown">
<a class="nav-link dropdown-toggle" href="#" id="offcanvasnavbarResources" role="button" data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">Resources  <img src="/assets/images/carat.svg" alt=""></a>
	
<div class="dropdown-menu" aria-labelledby="offcanvasnavbarResources">
<a class="dropdown-item" href="https://www.neotomadb.org/resources">Resources Overview</a>
				 	
<a class="dropdown-item" href="https://www.neotomadb.org/resources/proposal-preparation">Proposal Preparation</a>
<a class="dropdown-item dropdown-item-external" href="https://www.neotomadb.org/resources/neotomadb-publications">NeotomaDB Publications</a>
</div>
</li>

<!-- People -->
<li><a class="nav-link" href="/people" >People</a></li>

</ul>
	

<div class="search" role="search">
<form method="post" action="https://www.neotomadb.org/search/results">

<label for="q" class="header-label visually-hidden">Search</label>
<div class="d-flex align-items-center">
<input id="q" type="search" name="q" aria-label="Search" placeholder="Search NeotomaDB" maxlength="200">
  
<button name="submit" class="btn" type="submit" value="Submit" aria-label="Search Site"><span class="visually-hidden">Submit</span><span class="btn-search"><img src="/assets/images/search-icon.svg" alt="Magnifying Glass Search Button Icon"></span></button>
</div>

</form>
</div>


</div>
		
</div></div>   
</nav>
</div></div></div>
