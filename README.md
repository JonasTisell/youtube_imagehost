# YouTube Image Host URL Parameter Documentation
###### These are also usable in Picasa, Blogger and Google+ image links, as they all use the Google Image Host

## Rules

If image is 5000px*5000px, GIF will be disabled
Needs to have a slash in the end or all parameters will be ignored
Trying unexisting parameters makes the image 404
Highest quality saved on server is 797x797

## Default parameters (set in all profile images)

s - size, proceeded by a integer (defaults to 512x512 if not set - can also use w[size] and h[size])
k - Makes GIF show a play-button (if "no" isn't set)
no - Stops GIF from moving (needs "rj")
rj - makes image JPG (when not set, image gets changed to the original filetype)
c - makes width 2 pixels under for some reason (sometimes also allows image to be larger than 797x797 pixels)
c0xffffffff - Unknown
mo - Unknown

## Other parameters

g - Shows the XML used to render the profile picture (TileInfo) - also ignores other parameters
fcrop64 - Doesn't do anything on profile pictures, but setting it to 2 shows an alert-sign (from banner-parameters)
d - Autodownloads image (Credit to Codesiderations)
p - Makes the image bigger than the size, and crops it
a / mm - Shows the old default profile-picture (blue square with a star inside) - Always shows if parameter starts with mm (can have anything behind)
h (no int) - Puts img in a html-page
cc - Makes image circular (doesn't work if c is set)
I - Redirects url to googleusercontent.com - once redirected it shows client doesn't have permission. (removing I then makes it work)
U - Does same as -I, but url is different (removing U then makes it work)
ft - Unknown
t - Starting parameter with -t allows you to write anything after it without it breaking (e.g. "-tHELLO" won't break it)
