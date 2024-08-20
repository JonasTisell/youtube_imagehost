# YouTube Image Host URL Parameter Documentation
###### These are also usable in Picasa, Blogger and Google+ image links, as they all use the Google Image Host
###### Mostly accurate as of March 2023

## Rules

If GIF is bigger than 8192px*8192px, the image shows error code 400 (_Bad Request_) 

If image is bigger than 12247px*12247px, the image shows error code 400 (_Bad Request_) 

Trying unexisting parameters makes the image show error code 400 (_Bad Request_)

Highest quality saved on server is 797x797 for profile pictures from YouTube

## Default parameters (_set in all profile images and various others_)

s - size, proceeded by a integer (_defaults to 512x512 if not set - can also use w\[size] and h\[size]_)

k - Makes GIF show a play-button (_if "no" isn't set_)

no - Stops GIF from moving (_needs "rj"_)

rj - makes image JPG (_when not set, image gets changed to the original filetype_)

c - makes image same width and height, also makes width 2 pixels smaller sometimes, for some reason (_sometimes also allows image to be larger than 797x797 pixels_)

c0xffffffff - Unknown

mo - Unknown

## Other parameters

cc - Makes image circular (doesn't work if c is set)

d - Autodownloads image (_Credit to [Codesiderations](http://www.codesiderations.com/2017/02/09/blogger-amp-proxy.html)_)

fcrop64 - crops the image. Setting it to 2 throws an error (used to show an alert-sign)  [_from banner parameters_]

ft - Unknown

g - Shows the XML used to render the profile picture (_TileInfo_) - also ignores other parameters

h - Displays img in a html-page

I - Redirects url to googleusercontent.com - once redirected it shows client doesn't have permission. (_removing I then makes it work_)

l - compression level, proceeded by an integer (e.g. l0 results in a heavily compressed image) - default is around "l82", thus making "l100" higher quality than default [found in Youtube Music]

p - Crops the image to the width and height, instead of resizing to the smallest value. If only width or height is set alone, it malfunctions.

t - Starting parameter with -t allows you to write anything after it without it breaking (_e.g. "-tHELLO" won't break it_)

U - Does same as -I, but url is different (_removing U then makes it work_)

## Retired parameters (_no longer works_)

a / mm - Shows the old default profile-picture (_blue square with a star inside_) - Always shows if parameter starts with mm (_can have anything behind_)
