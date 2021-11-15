# Straight-Line-Road-Trip

Google Maps tends to return driving directions using the lowest total travel time (though it will occasionally give you a slightly higher travel time in exchange for less complexity). This is useful, and it's what I'm looking for a majority of the time, but it can become pretty boring on trips which are undertaken frequently, or which are just not very interesting. One solution I've come up with is the "straight-line road trip" -- this involves plotting the latitude and longitude of your origin point and destination, plotting equidistant points between them, and then asking Google Maps for instructions between those points. Using this method I've gone on many very remote and scenic roads I can't imagine ever being recommended to visit by anyone. Calculating this out is pretty tedious, though.

So I've written a script in Python that does this for you using the Selenium web scraper. It's in the form of a function where string1 is your origin point, string2 is your destination, and _n_ is how many lines between points you'd like (2 cuts the trip in half, with 1 point between your origin and destination; 3 cuts in thirds, and so forth). The maximum you can use is 9; any more than this and Google Maps won't work as intended.

The function returns a URL that can be copypasted manually.
