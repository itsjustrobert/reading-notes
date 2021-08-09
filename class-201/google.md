# What Google Learned From Its Quest to Build the Perfect Team

Like most 25-year-olds, Julia Rozovsky wasn’t sure what she wanted to do with her life. She had worked at a consulting firm, but it wasn’t a good match. Then she became a researcher for two professors at Harvard, which was interesting but lonely. Maybe a big corporation would be a better fit. Or perhaps a fast-growing start-up. All she knew for certain was that she wanted to find a job that was more social. ‘‘I wanted to be part of a community, part of something people were building together,’’ she told me. She thought about various opportunities — Internet companies, a Ph.D. program — but nothing seemed exactly right. So in 2009, she chose the path that allowed her to put off making a decision: She applied to business schools and was accepted by the Yale School of Management.

The fact that these insights aren’t wholly original doesn’t mean Google’s contributions aren’t valuable. In fact, in some ways, the ‘‘employee performance optimization’’ movement has given us a method for talking about our insecurities, fears and aspirations in more constructive ways. It also has given us the tools to quickly teach lessons that once took managers decades to absorb. Google, in other words, in its race to build the perfect team, has perhaps unintentionally demonstrated the usefulness of imperfection and done what Silicon Valley does best: figure out how to create psychological safety faster, better and in more productive ways.

‘‘Just having data that proves to people that these things are worth paying attention to sometimes is the most important step in getting them to actually pay attention,’’ Rozovsky told me. ‘‘Don’t underestimate the power of giving people a common platform and operating language.’’

Project Aristotle is a reminder that when companies try to optimize everything, it’s sometimes easy to forget that success is often built on experiences — like emotional interactions and complicated conversations and discussions of who we want to be and how our teammates make us feel — that can’t really be optimized. Rozovsky herself was reminded of this midway through her work with the Project Aristotle team. ‘‘We were in a meeting where I made a mistake,’’ Rozovsky told me. She sent out a note afterward explaining how she was going to remedy the problem. ‘‘I got an email back from a team member that said, ‘Ouch,’ ’’ she recalled. ‘‘It was like a punch to the gut. I was already upset about making this mistake, and this note totally played on my insecurities.’’

If this had happened earlier in Rozovsky’s life — if it had occurred while she was at Yale, for instance, in her study group — she probably wouldn’t have known how to deal with those feelings. The email wasn’t a big enough affront to justify a response. But all the same, it really bothered her. It was something she felt she needed to address.

# Transforms :

With CSS3 came new ways to position and alter elements. Now general layout techniques can be revisited with alternative ways to size, position, and change elements. All of these new techniques are made possible by the transform property.

The transform property comes in two different settings, two-dimensional and three-dimensional. Each of these come with their own individual properties and values.

Within this lesson we’ll take a look at both two-dimensional and three-dimensional transforms. Generally speaking, browser support for the transform property isn’t great, but it is getting better every day. For the best support vendor prefixes are encouraged, however you may need to download the nightly version of Chrome to see all of these transforms in action.

The actual syntax for the `transform` property is quite simple, including the transform property followed by the value. The value specifies the transform type followed by a specific amount inside parentheses.

> `div {`
>  ` -webkit-transform: scale(1.5);`
>      `-moz-transform: scale(1.5);`
>        `-o-transform: scale(1.5);`
>       `    transform: scale(1.5);`
> `}`

## 2D Transforms :

Elements may be distorted, or transformed, on both a two-dimensional plane or a three-dimensional plane. Two-dimensional transforms work on the x and y axes, known as horizontal and vertical axes. Three-dimensional transforms work on both the x and y axes, as well as the z axis. These three-dimensional transforms help define not only the length and width of an element, but also the depth. We’ll start by discussing how to transform elements on a two-dimensional plane, and then work our way into three-dimensional transforms.

# Transitions & Animations :

One evolution with CSS3 was the ability to write behaviors for transitions and animations. Front end developers have been asking for the ability to design these interactions within HTML and CSS, without the use of JavaScript or Flash, for years. Now their wish has come true.

With CSS3 transitions you have the potential to alter the appearance and behavior of an element whenever a state change occurs, such as when it is hovered over, focused on, active, or targeted.

Animations within CSS3 allow the appearance and behavior of an element to be altered in multiple keyframes. Transitions provide a change from one state to another, while animations can set multiple points of transition upon different keyframes.

## Transitions :

As mentioned, for a transition to take place, an element must have a change in state, and different styles must be identified for each state. The easiest way for determining styles for different states is by using the `:hover`, `:focus`, `:active`, and `:target` pseudo-classes.

There are four transition related properties in total, including `transition-property`, `transition-duration`, `transition-timing-function`, and `transition-delay`. Not all of these are required to build a transition, with the first three are the most popular.

In the example below the box will change its background color over the course of 1 second in a linear fashion.

## Animations :

Transitions do a great job of building out visual interactions from one state to another, and are perfect for these kinds of single state changes. However, when more control is required, transitions need to have multiple states. In return, this is where animations pick up where transitions leave off.

To set multiple points at which an element should undergo a transition, use the `@keyframes` rule. The `@keyframes` rule includes the animation name, any animation breakpoints, and the properties intended to be animated.