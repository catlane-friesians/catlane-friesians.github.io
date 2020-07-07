GET all the pohots using something like this:

     wget -nd -r -H -p -A jpg,jpeg,png,gif -e robots=off https://catlane.co.uk

Doesn't quite seem to work - doesn't collect everything

/https:\/\/farm([0-9]+)\.static.flickr.com\/([0-9]+)\/([0-9_a-z]+)\.jpg/g

Likely better to just fina all instances of

    /https:\/\/farm([0-9]+)\.static.flickr.com\/([0-9]+)\/([0-9_a-z]+)\.jpg/g

THen write a script to collect all , then rename the img src attributes in the pages.
