# P10-Points-In-A-File
Change the last program so that instead of working with two points, the program reads a list of five or more points from a file.

Create a file that has the data for at least five points.
  Each line in the file should have each point’s lat and lon coordinates and a description. It will look like this:
      35.07152486937333, -106.62857188674603, Main Campus
      35.13570178128822, -106.5191248669646, Montoya
      35.31819963442066, -106.68376032037753, Rio Rancho
      35.08572696704096, -106.64888652094055, STEMULUS Center
      35.183775418129066, -106.59364371114025, ATC

In the main part of your program do the following:
    a.	Create a list that you will use to collect the points. ( Something like pointList = [] ).
    b.	Read points in from a file.
    c.	As the program reads lat lon and description from the file, use those values to create a point and add that point to a List. 
        Something like: newPoint = GeoPoint(lat, lon, description)
                        pointList.append(newPoint)
    d.	Inside the “Do another (y/n)?” loop do the following:
          i.	  Ask the user for their location. 
          ii.	  Create a point to represent the user’s location. 
          iii.	Iterate through the point list and find the closest point. 
          iv. 	Tell the user which point they are closest to in this format:
                You are closest to <description> which is located at <point’s lat, lon coordinates>
          v.	  Ask “Do another (y/n)?” and loop if they respond with ‘y’
