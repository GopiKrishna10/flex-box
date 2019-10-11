# flex-box
Sample Flex Box Model
# Flex-grow and flex-shrink

The beauty of flex items is being “flexible.”

The flex-grow and flex-shrink properties allow us play around this “flexibility” even more.

The flex-grow and flex-shrink properties control how much a flex-item should “grow” (extend) if there are extra spaces, or “shrink” if there are no extra spaces.

They may take up any values ranging from 0 to any positive number. 0 || positive number

#Flex-basis

Remember how I said the beauty of the flex-items is being “flexible”? Well, it appears you also have a control over that.

The flex-basis property specifies the initial size of a flex-item. Before the flex-grow or flex-shrink properties adjust it's size to fit the container or not.

The previous statement is really important- so i’m taking a moment to reinforce that.

The default value is flex-basis: auto. Flex-basis can take on any values you'd use on the normal width property. That is, percentages || ems || rems || pixels etc

Note that when trying to set the basis property to a zero based value, use the unit also. Use flex-basis: 0px not just flex-basis: 0

I’d bring back the “one list” example here again.

<ul>    <li>I am a simple list</li></ul>

By default, the initial width of the flex item is influenced by the default value, flex-basis: auto.

The width of the flex-item is computed "automatically" based on the content size (and obviously, plus whatever padding you set too).

If, however, you want to set the flex-item to a fixed width, you can also do this:

li {    flex-basis: 150px;}
Now the flex-item has been constrained to a width of 150px.

# flex shorthand

The flex shorthand allows you set the flex-grow, flex-shrink and flex-basis properties all at once.

The acronym, GSB may help.
G - grow
S - shrink
B - basis

li {  flex: 0 1 auto;}

# Align-self

The align-self property takes a step further in giving us so much control over flex items.

You already saw how the align-items property helps in collectively aligning all flex-items within a flex-container.

What if you wanted to change the position of a single flex-item along the cross-axis, without affecting the neighboring flex-items?

This is where the align-self property comes to the rescue.

It may take on any of these values: auto || flex-start || flex-end || center || baseline || stretch

# Link related To Flex Box to understand for further

# https://www.freecodecamp.org/news/understanding-flexbox-everything-you-need-to-know-b4013d4dc9af/
