


# reviwe 

# Transforms


With CSS3 came new ways to position and alter elements. Now general layout techniques can be revisited with alternative ways to size, position, and change elements. All of these new techniques are made possible by the transform property.


The transform property comes in two different settings, two-dimensional and three-dimensional. Each of these come with their own individual properties and values.


Within this lesson we’ll take a look at both two-dimensional and three-dimensional transforms. Generally speaking, browser support for the transform property isn’t great, but it is getting better every day.


* ## Transform Syntax

The actual syntax for the transform property is quite simple, including the transform property followed by the value. The value specifies the transform type followed by a specific amount inside parentheses.


* ## 2D Transforms

Elements may be distorted, or transformed, on both a two-dimensional plane or a three-dimensional plane. Two-dimensional transforms work on the x and y axes, known as horizontal and vertical axes. Three-dimensional transforms work on both the x and y axes, as well as the z axis. These three-dimensional transforms help define not only the length and width of an element, but also the depth. We’ll start by discussing how to transform elements on a two-dimensional plane, and then work our way into three-dimensional transforms.

* 2D Rotate

The transform property accepts a handful of different values. The rotate value provides the ability to rotate an element from 0 to 360 degrees. Using a positive value will rotate an element clockwise, and using a negative value will rotate the element counterclockwise. The default point of rotation is the center of the element, 50% 50%, both horizontally and vertically. Later we will discuss how you can change this default point of rotation.


* 2D Scale

> Using the scale value within the transform property allows you to change the appeared size of an element. The default scale value is 1, therefore any value between .99 and .01 makes an element appear smaller while any value greater than or equal to 1.01 makes an element appear larger.


* 2D Translate

> The translate value works a bit like that of relative positioning, pushing and pulling an element in different directions without interrupting the normal flow of the document. Using the translateX value will change the position of an element on the horizontal axis while using the translateY value will change the position of an element on the vertical axis.

As with the scale value, to set both the x and y axis values at once, use the translate value and declare the x axis value first, followed by a comma, and then the y axis value.

##### The distance values used within the translate value may be any general length measurement, most commonly pixels or percentages. Positive values will push an element down and to the right of its default position while negative values will pull an element up and to the left of its default position. 


* 2D Skew
![fasfafafa](https://stackoverflow.com/questions/52115089/css-transform-rotate-skew-doesnt-work-together.jpg)
> The last transform value in the group, skew, is used to distort elements on the horizontal axis, vertical axis, or both. The syntax is very similar to that of the scale and translate values. Using the skewX value distorts an element on the horizontal axis while the skewY value distorts an element on the vertical axis. To distort an element on both axes the skew value is used, declaring the x axis value first, followed by a comma, and then the y axis value.%p

#### The distance calculation of the skew value is measured in units of degrees. Length measurements, such as pixels or percentages, do not apply here.


* ## Combining Transforms

> It is common for multiple transforms to be used at once, rotating and scaling the size of an element at the same time for example. In this event multiple transforms can be combined together. To combine transforms, list the transform values within the transform property one after the other without the use of commas.

#### Using multiple transform declarations will not work, as each declaration will overwrite the one above it. The behavior in that case would be the same as if you were to set the height of an element numerous times.


* ## Transform Origin

#### As previously mentioned, the default transform origin is the dead center of an element, both 50% horizontally and 50% vertically. To change this default origin position the transform-origin property may be used.

>The transform-origin property can accept one or two values. When only one value is specified, that value is used for both the horizontal and vertical axes. If two values are specified, the first is used for the horizontal axis and the second is used for the vertical axis.

*Individually the values are treated like that of a background image position, using either a length or keyword value. That said, 0 0 is the same value as top left, and 100% 100% is the same value as bottom right. More specific values can also be set, for example 20px 50px would set the origin to 20 pixels across and 50 pixels down the element.*


* ## Perspective

In order for three-dimensional transforms to work the elements need a perspective from which to transform. The perspective for each element can be thought of as a vanishing point, similar to that which can be seen in three-dimensional drawings.

> The perspective of an element can be set in two different ways. One way includes using the perspective value within the transform property on individual elements, while the other includes using the perspective property on the parent element residing over child elements being transformed.

`Using the perspective value within the transform property works great for transforming one element from a single, unique perspective. When you want to transform a group of elements all with the same perspective, or vanishing point, apply the perspective property to their parent element.`


* Perspective Depth Value

> The perspective value can be set as none or a length measurement. The none value turns off any perspective, while the length value will set the depth of the perspective. The higher the value, the further away the perspective appears, thus creating a fairly low intensity perspective and a small three-dimensional change. The lower the value the closer the perspective appears, thus creating a high intensity perspective and a large three-dimensional change.

#### Imagine yourself standing 10 feet away from a 10 foot cube as compared to standing 1,000 feet away from the same cube. At 10 feet, your distance to the cube is the same as the dimensions of the cube, therefore the perspective shift is much greater than it will be at 1,000 feet, where the dimensions of the cube are only one one-hundredth of your distance to the cube. The same thinking applies to perspective depth values.


* Perspective Origin

As with setting a transform-origin you can also set a perspective-origin. The same values used for the transform-origin property may also be used with the perspective-origin property, and maintain the same relationship to the element. The large difference between the two falls where the origin of a transform determines the coordinates used to calculate the change of a transform, while the origin of a perspective identifies the coordinates of the vanishing point of a transform.


* ## 3D Transforms

Working with two-dimensional transforms we are able to alter elements on the horizontal and vertical axes, however there is another axis along which we can transform elements. Using three-dimensional transforms we can change elements on the z axis, giving us control of depth as well as length and width.

* 3D Rotate

So far we’ve discussed how to rotate an object either clockwise or counterclockwise on a flat plane. With three-dimensional transforms we can rotate an element around any axes. To do so, we use three new transform values, including rotateX, rotateY, and rotateZ.

Using the rotateX value allows you to rotate an element around the x axis, as if it were being bent in half horizontally. Using the rotateY value allows you to rotate an element around the y axis, as if it were being bent in half vertically. Lastly, using the rotateZ value allows an element to be rotated around the z axis.

As with the general rotate value before, positive values will rotate the element around its dedicated axis clockwise, while negative values will rotate the element counterclockwise.


* 3D Scale

By using the scaleZ three-dimensional transform elements may be scaled on the z axis. This isn’t extremely exciting when no other three-dimensional transforms are in place, as there is nothing in particular to scale. In the demonstration below the elements are being scaled up and down on the z axis, however the rotateX value is added in order to see the behavior of the scaleZ value. When removing the rotateX in this case, the elements will appear to be unchanged.


* 3D Translate

Elements may also be translated on the z axis using the translateZ value. A negative value here will push an element further away on the z axis, resulting in a smaller element. Using a positive value will pull an element closer on the z axis, resulting in a larger element.

While this may appear to be very similar to that of the two-dimensional transform scale value, it is actually quite different. The transform is taking place on the z axis, not the x or y axes. When working with three-dimensional transforms, being able to move an element on the z axis does have great benefits


* 3D Skew

Skew is the one two-dimensional transform that cannot be transformed on a three-dimensional scale. Elements may be skewed on the x and y axis, then transformed three-dimensionally as wished, but they cannot be skewed on the z axis.


* ## Transform Style

On occasion three-dimensional transforms will be applied on an element that is nested within a parent element which is also being transformed. In this event, the nested, transformed elements will not appear in their own three-dimensional space. To allow nested elements to transform in their own three-dimensional plane use the transform-style property with the preserve-3d value.

The transform-style property needs to be placed on the parent element, above any nested transforms. The preserve-3d value allows the transformed children elements to appear in their own three-dimensional plane while the flat value forces the transformed children elements to lie flat on the two-dimensional plane.


* ## Backface Visibility

When working with three-dimensional transforms, elements will occasionally be transformed in a way that causes them to face away from the screen. This may be caused by setting the rotateY(180deg) value for example. By default these elements are shown from the back. So if you prefer not to see these elements at all, set the backface-visibility property to hidden, and you will hide the element whenever it is facing away from the screen.

The other value to backface-visibility is visible which is the default value, always displaying an element, no matter which direction it faces.

In the demonstration below notice how the second box isn’t displayed because backface-visibility: hidden; declaration has been set. The backface-visibility property takes even more significance when using animations.


# Transitions & Animations

> One evolution with CSS3 was the ability to write behaviors for transitions and animations. Front end developers have been asking for the ability to design these interactions within HTML and CSS, without the use of JavaScript or Flash, for years. Now their wish has come true.

`With CSS3 transitions you have the potential to alter the appearance and behavior of an element whenever a state change occurs, such as when it is hovered over, focused on, active, or targeted.`

### Animations within CSS3 allow the appearance and behavior of an element to be altered in multiple keyframes. Transitions provide a change from one state to another, while animations can set multiple points of transition upon different keyframes.

* ## Transitions

> As mentioned, for a transition to take place, an element must have a change in state, and different styles must be identified for each state. The easiest way for determining styles for different states is by using the :hover, :focus, :active, and :target pseudo-classes.

There are four transition related properties in total, including transition-property, transition-duration, transition-timing-function, and transition-delay. Not all of these are required to build a transition, with the first three are the most popular.

* Transitional Property

The transition-property property determines exactly what properties will be altered in conjunction with the other transitional properties. By default, all of the properties within an element’s different states will be altered upon change. However, only the properties identified within the transition-property value will be affected by any transitions.

In the example above, the background property is identified in the transition-property value. Here the background property is the only property that will change over the duration of 1 second in a linear fashion. Any other properties included when changing an element’s state, but not included within the transition-property value, will not receive the transition behaviors as set by the transition-duration or transition-timing-function properties.

If multiple properties need to be transitioned they may be comma separated within the transition-property value. Additionally, the keyword value all may be used to transition all properties of an element.


* Transitional Properties

It is important to note, not all properties may be transitioned, only properties that have an identifiable halfway point. Colors, font sizes, and the alike may be transitioned from one value to another as they have recognizable values in-between one another. The display property, for example, may not be transitioned as it does not have any midpoint. A handful of the more popular transitional properties include the following.

    background-color
    background-position
    border-color
    border-width
    border-spacing
    bottom
    clip
    color
    crop
    font-size
    font-weight
    height
    left
    letter-spacing
    line-height
    margin
    max-height
    max-width
    min-height
    min-width
    opacity
    outline-color
    outline-offset
    outline-width
    padding
    right
    text-indent
    text-shadow
    top
    vertical-align
    visibility
    width
    word-spacing
    z-index


* Transition Duration

The duration in which a transition takes place is set using the transition-duration property. The value of this property can be set using general timing values, including seconds (s) and milliseconds (ms). These timing values may also come in fractional measurements, .2s for example.

When transitioning multiple properties you can set multiple durations, one for each property. As with the transition-property property value, multiple durations can be declared using comma separated values. The order of these values when identifying individual properties and durations does matter. For example, the first property identified within the transition-property property will match up with the first time identified within the transition-duration property, and so forth.

If multiple properties are being transitioned with only one duration value declared, that one value will be the duration of all the transitioned properties.


* Transition Timing

The transition-timing-function property is used to set the speed in which a transition will move. Knowing the duration from the transition-duration property a transition can have multiple speeds within a single duration. A few of the more popular keyword values for the transition-timing-function property include linear, ease-in, ease-out, and ease-in-out.

The linear keyword value identifies a transition moving in a constant speed from one state to another. The ease-in value identifies a transition that starts slowly and speeds up throughout the transition, while the ease-out value identifies a transition that starts quickly and slows down throughout the transition. The ease-in-out value identifies a transition that starts slowly, speeds up in the middle, then slows down again before ending.

Each timing function has a cubic-bezier curve behind it, which can be specifically set using the cubic-bezier(x1, y1, x2, y2) value. Additional values include step-start, step-stop, and a uniquely identified steps(number_of_steps, direction) value.

When transitioning multiple properties, you can identify multiple timing functions. These timing function values, as with other transition property values, may be declared as comma separated values.


* ## Animations
![jhdfjshdf](https://www.bypeople.com/wp-content/uploads/2019/01/css-animation-101-featured.jpg)
Transitions do a great job of building out visual interactions from one state to another, and are perfect for these kinds of single state changes. However, when more control is required, transitions need to have multiple states. In return, this is where animations pick up where transitions leave off.

* Animations Keyframes

To set multiple points at which an element should undergo a transition, use the @keyframes rule. The @keyframes rule includes the animation name, any animation breakpoints, and the properties intended to be animated.


* Animation Name

Once the keyframes for an animation have been declared they need to be assigned to an element. To do so, the animation-name property is used with the animation name, identified from the @keyframes rule, as the property value. The animation-name declaration is applied to the element in which the animation is to be applied to.


* Animation Duration, Timing Function, & Delay

Once you have declared the animation-name property on an element, animations behave similarly to transitions. They include a duration, timing function, and delay if desired. To start, animations need a duration declared using the animation-duration property. As with transitions, the duration may be set in seconds or milliseconds.

A timing function and delay can be declared using the animation-timing-function and animation-delay properties respectively. The values for these properties mimic and behave just as they do with transitions.


* ## Customizing Animations

Animations also provide the ability to further customize an element’s behavior, including the ability to declare the number of times an animation runs, as well as the direction in which an animation completes.

* Animation Iteration

By default, animations run their cycle once from beginning to end and then stop. To have an animation repeat itself numerous times the animation-iteration-count property may be used. Values for the animation-iteration-count property include either an integer or the infinite keyword. Using an integer will repeat the animation as many times as specified, while the infinite keyword will repeat the animation indefinitely in a never ending fashion.


* Animation Direction

> On top of being able to set the number of times an animation repeats, you may also declare the direction an animation completes using the animation-direction property. Values for the animation-direction property include normal, reverse, alternate, and alternate-reverse.

> The normal value plays an animation as intended from beginning to end. The reverse value will play the animation exactly opposite as identified within the @keyframes rule, thus starting at 100% and working backwards to 0%.

##### The alternate value will play an animation forwards then backwards. Within the keyframes that includes running forward from 0% to 100% and then backwards from 100% to 0%. Using the animation-iteration-count property may limit the number of times an animation runs both forwards and backwards. The count starts at 1 running an animation forwards from 0% to 100%, then adds 1 running an animation backwards from 100% to 0%. Combining for a total of 2 iterations. The alternate value also inverses any timing functions when playing in reverse. If an animation uses the ease-in value going from 0% to 100%, it then uses the ease-out value going from 100% to 0%.

> Lastly, the alternate-reverse value combines both the alternate and reverse values, running an animation backwards then forwards. The alternate-reverse value starts at 100% running to 0% and then back to 100% again.

* Animation Play State

The animation-play-state property allows an animation to be played or paused using the running and paused keyword values respectively. When you play a paused animation, it will resume running from its current state rather than starting from the very beginning again.

* Animation Fill Mode

#### The animation-fill-mode property identifies how an element should be styled either before, after, or before and after an animation is run. The animation-fill-mode property accepts four keyword values, including none, forwards, backwards, and both.

> The none value will not apply any styles to an element before or after an animation has been run.

The forwards value will keep the styles declared within the last specified keyframe. These styles may, however, be affected by the animation-direction and animation-iteration-count property values, changing exactly where an animation ends.

The backwards value will apply the styles within the first specified keyframe as soon as being identified, before the animation has been run. This does include applying those styles during any time that may be set within an animation delay. The backwards value may also be affected by the animation-direction property value.

Lastly, the both value will apply the behaviors from both the forwards and backwards values.


# simple transition

* Fade in

Having things fade in is a fairly common request from clients. It’s a great way to emphasize functionality or draw attention to a call to action.

Fade in effects are coded in two steps: first, you set the initial state; next, you set the change.

* Change color

> Animating a change of color used to be unbelievably complex, with all kinds of math involved in calculating separate RGB values and then recombining them. Now, we just set the div’s class to “color” and specify the color we want in our CSS. 


* Grow & Shrink

> To grow an element, you used to have to use its width and height, or its padding. But now we can use CSS3’s transform to enlarge.

Shrinking an element is as simple as growing it. To enlarge an element we specify a value greater than 1, to shrink it, we specify a value less than 1


* Swing

> Not all elements use the transition property. We can also create highly complex animations using @keyframes, animation and animation-iteration.

In this case, we’ll first define a CSS animation in your styles. You’ll notice that due to implementation issues, we need to use @-webkit-keyframes as well as @keyframes. 


* Inset border

>One of the hottest button styles right now is the ghost button; a button with no background and a heavy border. We can of course add a border to an element simply, but that will change the element’s position. We could fix that problem using box sizing, but a far simpler solution is the transition in a border using an inset box shadow.



--------------------------------------------------------------------------------------------------------------------





# What Google Learned From Its Quest to Build the Perfect Team
## Story with benefit softskils 

> the sroty told us about: 25-year-olds, Julia Rozovsky wasn’t sure what she wanted to do with her life. She had worked at a consulting firm, but it wasn’t a good match. Then she became a researcher for two professors at Harvard, which was interesting but lonely. Maybe a big corporation would be a better fit. Or perhaps a fast-growing start-up. All she knew for certain was that she wanted to find a job that was more social. ‘‘I wanted to be part of a community, part of something people were building together,’’ she told me. She thought about various opportunities — Internet companies, a Ph.D. program — but nothing seemed exactly right. So in 2009, she chose the path that allowed her to put off making a decision: She applied to business schools and was accepted by the Yale School of Management.


#### When Rozovsky arrived on campus, she was assigned to a study group carefully engineered by the school to foster tight bonds. Study groups have become a rite of passage at M.B.A. programs, a way for students to practice working in teams and a reflection of the increasing demand for employees who can adroitly navigate group dynamics. A worker today might start the morning by collaborating with a team of engineers, then send emails to colleagues marketing a new brand, then jump on a conference call planning an entirely different product line, while also juggling team meetings with accounting and the party-planning committee. To prepare students for that complex world, business schools around the country have revised their curriculums to emphasize team-focused learning.


> Every day, between classes or after dinner, Rozovsky and her four teammates gathered to discuss homework assignments, compare spreadsheets and strategize for exams. Everyone was smart and curious, and they had a lot in common: They had gone to similar colleges and had worked at analogous firms. These shared experiences, Rozovsky hoped, would make it easy for them to work well together. But it didn’t turn out that way. ‘‘There are lots of people who say some of their best business-school friends come from their study groups,’’ Rozovsky told me. ‘‘It wasn’t like that for me.’’


> Instead, Rozovsky’s study group was a source of stress. ‘‘I always felt like I had to prove myself,’’ she said. The team’s dynamics could put her on edge. When the group met, teammates sometimes jockeyed for the leadership position or criticized one another’s ideas. There were conflicts over who was in charge and who got to represent the group in class. ‘‘People would try to show authority by speaking louder or talking over each other,’’ Rozovsky told me. ‘‘I always felt like I had to be careful not to make mistakes around them.’’

![ksmsmfs](https://static01.nyt.com/images/2016/02/28/magazine/28mag-teams2/28mag-teams2-superJumbo.jpg?quality=90&auto=webp.jpg)


> One of her favorite competitions asked teams to come up with a new business to replace a student-run snack store on Yale’s campus. Rozovsky proposed a nap room and selling earplugs and eyeshades to make money. Someone else suggested filling the space with old video games. There were ideas about clothing swaps. Most of the proposals were impractical, but ‘‘we all felt like we could say anything to each other,’’ Rozovsky told me. ‘‘No one worried that the rest of the team was judging them.’’ Eventually, the team settled on a plan for a micro­gym with a handful of exercise classes and a few weight machines. They won the competition. (The micro­gym — with two stationary bicycles and three treadmills — still exists.)

<!-- 
`Rozovsky’s study group dissolved in her second semester (it was up to the students whether they wanted to continue). Her case team, however, stuck together for the two years she was at Yale.` -->

<!-- It always struck Rozovsky as odd that her experiences with the two groups were dissimilar. Each was composed of people who were bright and outgoing. When she talked one on one with members of her study group, the exchanges were friendly and warm. It was only when they gathered as a team that things became fraught. By contrast, her case-competition team was always fun and easygoing. In some ways, the team’s members got along better as a group than as individual friends.

`I couldn’t figure out why things had turned out so different,’’ Rozovsky told me. ‘‘It didn’t seem like it had to happen that way.` -->


#### THE MOST IMPORTANT THINGS Our data-saturated age enables us to examine our work habits and office quirks with a scrutiny that our cubicle-bound forebears could only dream of. Today, on corporate campuses and within university laboratories, psychologists, sociologists and statisticians are devoting themselves to studying everything from team composition to email patterns in order to figure out how to make employees into faster, better and more productive versions of themselves. ‘‘We’re living through a golden age of understanding personal productivity,’’ says Marshall Van Alstyne, a professor at Boston University who studies how people share information. ‘‘All of a sudden, we can pick apart the small choices that all of us make, decisions most of us don’t even notice, and figure out why some people are so much more effective than everyone else.’’




The company’s top executives long believed that building the best teams meant combining the best people. They embraced other bits of conventional wisdom as well, like ‘‘It’s better to put introverts together,’’ said Abeer Dubey, a manager in Google’s People Analytics division, or ‘‘Teams are more effective when everyone is friends away from work.’’ But, Dubey went on, ‘‘it turned out no one had really studied which of those were true.’’








*No matter how researchers arranged the data, though, it was almost impossible to find patterns — or any evidence that the composition of a team made any difference. ‘‘We looked at 180 teams from all over the company,’’ Dubey said. `We had lots of data, but there was nothing showing that a mix of specific personality types or skills or backgrounds made any difference. The ‘who’ part of the equation didn’t seem to matter.` *





![sfsfsfsfs](https://static01.nyt.com/images/2016/02/28/magazine/28mag-teams3/28mag-teams3-superJumbo.jpg?quality=90&auto=webp.jpg)






##### What interested the researchers most, however, was that teams that did well on one assignment usually did well on all the others. Conversely, teams that failed at one thing seemed to fail at everything. The researchers eventually concluded that what distinguished the ‘‘good’’ teams from the dysfunctional groups was how teammates treated one another. The right norms, in other words, could raise a group’s collective intelligence, whereas the wrong norms could hobble a team, even if, individually, all the members were exceptionally bright.


#### But what was confusing was that not all the good teams appeared to behave in the same ways. `Some teams had a bunch of smart people who figured out how to break up work evenly,` said Anita Woolley, the study’s lead author. ‘‘Other groups had pretty average members, but they came up with ways to take advantage of everyone’s relative strengths. Some groups had one strong leader. Others were more fluid, and everyone took a leadership role.’’





*In other words, if you are given a choice between the serious-minded Team A or the free-flowing Team B, you should probably opt for Team B. Team A may be filled with smart people, all optimized for peak individual efficiency. But the group’s norms discourage equal speaking; there are few exchanges of the kind of personal information that lets teammates pick up on what people are feeling or leaving unsaid. There’s a good chance the members of Team A will continue to act like individuals once they come together, and there’s little to suggest that, as a group, they will become more collectively intelligent.*











>There was nothing in the survey that instructed Sakaguchi to share his illness with the group. There was nothing in Project Aristotle’s research that said that getting people to open up about their struggles was critical to discussing a group’s norms. But to Sakaguchi, it made sense that psychological safety and emotional conversations were related. The behaviors that create psychological safety — conversational turn-taking and empathy — are part of the same unwritten rules we often turn to, as individuals, when we need to establish a bond. And those human bonds matter as much at work as anywhere else. In fact, they sometimes matter more.





##### What Project Aristotle has taught people within Google is that no one wants to put on a ‘‘work face’’ when they get to the office. No one wants to leave part of their personality and inner life at home. But to be fully present at work, to feel ‘‘psychologically safe,’’ we must know that we can be free enough, sometimes, to share the things that scare us without fear of recriminations. We must be able to talk about what is messy or sad, to have hard conversations with colleagues who are driving us crazy. We can’t be focused just on efficiency. Rather, when we start the morning by collaborating with a team of engineers and then send emails to our marketing colleagues and then jump on a conference call, we want to know that those people really hear us. We want to know that work is more than just labor.


##### Which isn’t to say that a team needs an ailing manager to come together. Any group can become Team B. Sakaguchi’s experiences underscore a core lesson of Google’s research into teamwork: By adopting the data-driven approach of Silicon Valley, Project Aristotle has encouraged emotional conversations and discussions of norms among people who might otherwise be uncomfortable talking about how they feel. ‘‘Googlers love data,’’ Sakaguchi told me. But it’s not only Google that loves numbers, or Silicon Valley that shies away from emotional conversations. Most work­places do. ‘‘By putting things like empathy and sensitivity into charts and data reports, it makes them easier to talk about,’’ Sakaguchi told me. ‘‘It’s easier to talk about our feelings when we can point to a number.’’


##### Sakaguchi knows that the spread of his cancer means he may not have much time left. His wife has asked him why he doesn’t quit Google. At some point, he probably will. But right now, helping his team succeed ‘‘is the most meaningful work I’ve ever done,’’ he told me. He encourages the group to think about the way work and life mesh. Part of that, he says, is recognizing how fulfilling work can be. Project Aristotle ‘‘proves how much a great team matters,’’ he said. ‘‘Why would I walk away from that? Why wouldn’t I spend time with people who care about me?’’


*The technology industry is not just one of the fastest growing parts of our economy; it is also increasingly the world’s dominant commercial culture. And at the core of Silicon Valley are certain self-mythologies and dictums: Everything is different now, data reigns supreme, today’s winners deserve to triumph because they are cleareyed enough to discard yesterday’s conventional wisdoms and search out the disruptive and the new.*

