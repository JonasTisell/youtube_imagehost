# YouTube Image Host URL Parameter Documentation
###### These are also usable in Picasa, Blogger and Google+ image links, as they all use the Google Image Host
###### Mostly accurate as of June 2026

These parameters are separated by dashes, after the equals sign at the end of the URL.

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

c - while neither w and h is not set, or only one of them are set, it crops to 1:1 aspect ratio (square). If both w and h is set, it crops to the desired width/height.

c0x - Sets background color, especially useful if used with _cc_. (e.g _c0xff0000_ gives you a red background color)

mo - Unknown

## Other parameters

cc - Makes image circular (doesn't work if c is set)

d - Autodownloads the original image, ignores all other params (_Credit to [Codesiderations](http://www.codesiderations.com/2017/02/09/blogger-amp-proxy.html)_)

fcrop64 - crops the image. Setting it to 2 throws an error (used to show an alert-sign)  [_from banner parameters_]

ft - Unknown

g - Shows the XML used to render the profile picture (_TileInfo_) - also ignores other parameters

h - Displays img in a html-page

I - Redirects url to googleusercontent.com - once redirected it shows client doesn't have permission. (_removing I then makes it work_)

l - compression level, proceeded by an integer (e.g. l0 results in a heavily compressed image) - default is around "l82", thus making "l100" higher quality than default [found in Youtube Music]

p - Crops the image to the width and height, instead of resizing to the smallest value. If only width or height is set alone, it malfunctions. Without width and height set, it crops to a square slightly left of center. Ignores _cc_ 

t - Starting parameter with -t allows you to write anything after it without it breaking (_e.g. "-tHELLO" won't break it_)

U - Does same as -I, but url is different (_removing U then makes it work_)

## Retired parameters (_no longer works_)

a / mm - Shows the old default profile-picture (_blue square with a star inside_) - Always shows if parameter starts with mm (_can have anything behind_)
