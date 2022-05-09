# YouTube Image Host URL Parameter Documentation
###### These are also usable in Picasa, Blogger and Google+ image links, as they all use the Google Image Host

## Rules

If image is 5000px*5000px, GIF will be disabled

Needs to have a slash in the end or all parameters will be ignored

Trying unexisting parameters makes the image 404

Highest quality saved on server is 797x797 (for images from YouTube)

## Default parameters (_set in all profile images and various others_)

s - size, proceeded by a integer (_defaults to 512x512 if not set - can also use w\[size] and h\[size]_)

k - Makes GIF show a play-button (_if "no" isn't set_)

no - Stops GIF from moving (_needs "rj"_)

rj - makes image JPG (_when not set, image gets changed to the original filetype_)

c - makes width 2 pixels smaller for some reason (_sometimes also allows image to be larger than 797x797 pixels_)
c0xffffffff - Unknown
mo - Unknown

## Other parameters

g - Shows the XML used to render the profile picture (_TileInfo_) - also ignores other parameters

fcrop64 - Doesn't do anything on profile pictures, but setting it to 2 shows an alert-sign (_from banner-parameters_)

d - Autodownloads image (_Credit to Codesiderations_)

p - Makes the image bigger than the size, and crops it

a / mm - Shows the old default profile-picture (blue square with a star inside) - Always shows if parameter starts with mm (can have anything behind)

h (no int) - Puts img in a html-page

cc - Makes image circular (doesn't work if c is set)

I - Redirects url to googleusercontent.com - once redirected it shows client doesn't have permission. (_removing I then makes it work_)

U - Does same as -I, but url is different (_removing U then makes it work_)

ft - Unknown

t - Starting parameter with -t allows you to write anything after it without it breaking (_e.g. "-tHELLO" won't break it_)
