# outline

- https://alpha.inkscape.org/vectors/www.inkscapeforum.com/viewtopic57ab.html?t=34119

Inkscape This is a read-only archive of the inkscapeforum.com site. You can search for info here or post new questions and comments at inkscape.org/forums
InkscapeForum.com

An Inkscape users' forum

Skip to content
Advanced search
Border only towards the outside
Forum rules
Post Reply
7 posts • Page 1 of 1

mar_gian60
Posts: 5
Joined: Thu Sep 27, 2018 8:25 pm

Border only towards the outside

    Quote

Postby mar_gian60 » Sun Oct 14, 2018 7:55 pm
Hi,
when I assign a border to an object, such as a text, the border it expands towards the object and to the exterior of the object. Would it be possible to make it expand only towards the outside?
Thanks
Regards
Marco
Top

tylerdurden
Posts: 2344
Joined: Sun Apr 14, 2013 12:04 pm
Location: Michigan, USA

Re: Border only towards the outside

    Quote

Postby tylerdurden » Mon Oct 15, 2018 2:13 am
The fill and stroke dialog has tools for "paint order" which provide the ability to place the fill in front of the stroke, so that only the half of the stroke outside the path is shown.

paint-order.png
paint-order.png (11.77 KiB) Viewed 1584 times

Have a nice day.

I'm using Inkscape 0.92.2 (5c3e80d, 2017-08-06), 64 bit win8.1

The Inkscape manual has lots of helpful info! http://tavmjong.free.fr/INKSCAPE/MANUAL/html/
Top

User avatar
brynn
Posts: 10309
Joined: Wed Sep 26, 2007 4:34 pm
Location: western USA
Contact: Contact brynn

Re: Border only towards the outside

    Quote

Postby brynn » Mon Oct 15, 2018 9:46 pm
That's been a requested feature for a long time, but still not possible. Besides tylerdurden's suggestion, another suggestion would be to make the outline into a separate object.

There are probably a couple of ways to do that. Since I'm not sure if you might already know how, I'll wait for you to ask before I explain.
Basics - Help menu > Tutorials
Manual - Inkscape: Guide to a Vector Drawing Program
Inkscape Community - Inkscape FAQ - Gallery
Inkscape for Cutting Design
Top

mar_gian60
Posts: 5
Joined: Thu Sep 27, 2018 8:25 pm

Re: Border only towards the outside

    Quote

Postby mar_gian60 » Mon Oct 15, 2018 10:04 pm
Hi,

Thanks for your answers
I use inkscape in linux mint 18, and in the fill and stroke window, the order option not there is. But in windows 8.1 I have found it.
This is possible?
Instead regarding the suggestion of brynn, I have no idea how to do it.
I would be happy if you could give me some indication.
Thanks to both of the tips
Marco
Top

Moini
Posts: 3381
Joined: Mon Oct 05, 2015 10:44 am

Re: Border only towards the outside

    Quote

Postby Moini » Mon Oct 15, 2018 10:45 pm
Linux Mint 18 only provides an older version of Inkscape by default. But you can use the ppa instead:
https://launchpad.net/~inkscape.dev/+ar ... ntu/stable
Something doesn't work? - Keeping an eye on the status bar can save you a lot of time!

Inkscape FAQ - Learning Resources - Website with tutorials (German and English)
Top

mar_gian60
Posts: 5
Joined: Thu Sep 27, 2018 8:25 pm

Re: Border only towards the outside

    Quote

Postby mar_gian60 » Thu Oct 18, 2018 10:46 pm
THANKS!!!
Top

User avatar
brynn
Posts: 10309
Joined: Wed Sep 26, 2007 4:34 pm
Location: western USA
Contact: Contact brynn

Re: Border only towards the outside

    Quote

Postby brynn » Fri Oct 19, 2018 6:49 am
There are a couple of ways to make the stroke into a separate object.

1 - duplicate the object (Edit menu > Duplicate, or this button Image or there's probably a key shortcut, search at Help menu > Key and Mouse Ref)
2 - for the original object (which is now underneath the duplicate) remove the stroke, leaving only the fill color
3 - for the duplicate, remove the fill color, leaving only the stroke
4 - select the duplicate (on top) and do Path menu > Stroke to path (this changes the stroke into a path)
5 - switch to the Node tool :tool_node: and you can see the nodes for this new path
6 - set up Snapping (along the right edge of the window) like I have showing in the attached screenshot - this will make nodes snap to nodes

snap-basic.png
snap-basic.png (5.32 KiB) Viewed 1428 times

7 - using the Node tool, drag the inner nodes and snap them to the nodes on the original object, which is still showing there

Other way:

1 - duplicate the object
2 - for the original object on the bottom, remove the fill color, leaving only the stroke
3 - for the duplicate on top, remove the stroke, leaving only the fill color
4 - duplicate the top one again
5 - select the one on top and the one on the bottom (don't select the one in the middle) (let us know if you need instructions for this)
6 - Path menu > Difference
Basics - Help menu > Tutorials
Manual - Inkscape: Guide to a Vector Drawing Program
Inkscape Community - Inkscape FAQ - Gallery
Inkscape for Cutting Design
Top
Post Reply
7 posts • Page 1 of 1

Return to “Help with using Inkscape”
Jump to
Powered by phpBB® Forum Software © phpBB Limited
