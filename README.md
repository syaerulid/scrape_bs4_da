# Scraping Glints Website for Role Data Analyst

In this project, I want to learn about Data Collection, because it's <b>important part as a Data Analyst</b>
<br>
In this project I scrape data using <b>Python</b> languange
<br>
in the scraping process i use some of python library such:
<ol>
  <li>requests</li>
  <li>BeautifulSoup</li>
  <li>csv</li>
</ol>
<br>
<b>Objective:</b>
<br>
In this project, the objective is to determine the most common locations for Data Analyst jobs in Indonesia
<br>
with their range of salary and minimum experience
<br>
<br>
<b>Steps that I take:</b>
<br>
<ul>
  <li>I make a requests to Glints website, Inspect Element the glints page that i want to scrape to getting the correct method to perform requests</li>
  <li>I don't use Header: User Agents because they send Response 200, after I ask for requests</li>
  <li>Using beautifulsoup and 'html.parser' to parsing html content</li>
  <li>Inspect element to getting a container class in the div section</li>
  <li>using for loops and specific class_ to extract information that i need inside container class</li>
</ul>
<br>
<h1 align="center"><b>Problems that I encountered</b></h1>
<br><br>
<b>Scraping Data:</b>
<ul>
  <li>Location, Salary and Experience have the same class</li>
  <li>Location and Salary have <b>"span"</b></li>
  <li>Experience is the last elements in "div" but doesn't have any specific counter like span, that's why its printed Location, Salary and Experience when i iterate even i use [-1] as last</li>
  <li>I will do better next time to fix them, but i think its okay for now</li>
</ul>
<br><br>
<b>Saving Data to CSV:</b>
<ul>
  <li>for each loops i using <b>"print function"</b> to show the temporary results</li>
  <li>I created empty list name data = []</li>
  <li>but, when i try to append using data.append(variable_name), instead of iterate [i], they performs duplicate operation or they not iterate at all, and only print single value</li>
  <li>after searching for hours, i try to create specific empty list for each for loops like roles = [], companies = [], etc.</li>
  <li>and then i combine the list using zip function</li>
  
</ul>
<br>
<br>
<b>Outcome:</b>
<ul>
  <li>Saving file to CSV to perform further analysis</li>
</ul>
