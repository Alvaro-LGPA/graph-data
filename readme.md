1. Start by creating the train network as a weighted and directed Graph instance and assigning it to `trainNetwork`.


2. We just got funding to build out 6 train stations. Using the graph’s `.addVertex()` method, add the following station vertices to our `trainNetwork` with the names:

* Los Angeles
* San Francisco
* New York
* Atlanta
* Denver
* Calgary



3. We only want to service the routes our customers will travel the most, so let’s use `.addEdge()` to add the following route edges to the graph:

* From San Francisco to Los Angeles, which is 400mi
* From Los Angeles to San Francisco, which is 400mi
* From New York to Denver, which is 1800mi
* From Denver to New York, which is 1800mi
* From Calgary to Denver, which is 1000mi
* From Denver to Calgary, which is 1000mi
* From Los Angeles to Atlanta, which is 2100mi
* From Atlanta to Los Angeles, which is 2100mi



4. Darn! As we were building out our routes, there was a huge snowstorm that hit Calgary and New York. We were able to salvage the route from Denver to New York, but all of the routes to and from Calgary broke down.<br>
Using the graph’s `.removeEdge()` and `.removeVertex()` methods, remove the route from New York to Denver, all the routes to and from Calgary, and the Calgary station.
<br>

5. We’re finally all aboard the same page. Print out our final graph and check that we built the following routes:<br>
* San Francisco to and from Los Angeles
* Los Angeles to and from Atlanta
* Denver to New York
  
This wraps up our graph implementation! There are still some edge (pardon the pun) cases that we have not yet accounted for. If you’re feeling up for it, try to challenge yourself with the following:
<br>
* Currently, it is possible to add duplicate edges between two vertices. How will you improve this `Graph` implementation to avoid adding duplicate edges?
* How would you iterate through a directed graph? What about an undirected graph?
* How would you create a cycle with a directed graph?