Resizing Rectangle alters stroke widths

    #1
    KimJ KimJ @KimJ
    2019-12-01

    Hello,

    I've read through a few forum posts with similar questions, and I've checked to make sure the correct icon has been selected: "When scaling objects, scale the stroke width by the same proportion" is not working.

    I've also gone into Properties and checked under: Behavior/Transform "Scale stroke width" and "Preserved" under store transformation.

    The stroke width is still messed up when I resize the rectangle (manually or by adjusting the numerical size)

    Thank you! Any advice is appreciated:)
    #2
    brynn brynn @brynn
    2019-12-01

    Welcome to the forum!

    For Preferences > Behavior > Transform, it's probably better to keep it on Optimized.  That setting does not do what you're thinking it does.

    If you change it to Optimize and you still see the problem, could you show us in an SVG file, like with before and after?  Also, tell us exactly which steps you take, using which tools.

    I'm thinking maybe what you think is a stroke might be the actual object.  But we would need to see the SVG file, to really give correct suggestions.  You can attach it to this message, if you like, or upload it anywhere and give us the link to it.

    One thing you can check, if you're using the Pen tool, make sure it's set for Regular Bezier Path, and the Shape dropdown menu is set for None.  (Those settings are on the control bar, which is the first bar above the horizontal ruler.)
