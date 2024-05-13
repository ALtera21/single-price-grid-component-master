# Frontend Mentor - Single price grid component solution

This is a solution to the [Single price grid component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/single-price-grid-component-5ce41129d0ff452fec5abbbc). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)
  -[Author](#Author)

## Overview

I already did this 2 times before and this is my 3th times, i never submitted the last 2 cuz it is ugly
Hope it helps, thanks (and sorry for the bad english).

and thank you for looking at my projects, this is my second real project that i uploaded online.

### The challenge

Users should be able to:

- View the optimal layout for the component depending on their device's screen size
- See a hover state on desktop for the Sign Up call-to-action

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

Since this is my third time doing this, my code is cleaner than the first 2 attempts
1.) i created the layout in html, i divided it into 4 parts
-the main container(.container)
-the whitebox (.whiteBox)
-the left blue box (.left-blue-box)
-the right blue box (.right-blue-box)

1.)i made the body into flexbox so that the container could stand on the middle of the screen using {justify-content: center;}

2.) i styled all the the parts and used {box-sizing: border-box;} to make the size consistent
then i add {border: 2px solid black;} so that i can see the layout, the other reason to used the {box-sizing: border-box;}
is to padding the contents all at once, this also made the the section inside the container to pad on the right
but since it is border box, the size will become consistent.

3.) the rest is just styling it like normal, then i delete the {border: 2px solid black;}

4.) as for the right blue box's content, at first i thought of using <ol> and then delete the list's bullets
using {list-style: none;}, but it automatically pad to the right 20px relative with the already pad to the right
"right blue box sub header", basically it means that the list now pad to right by 40px instead of 20px,
so first i added {padding-left: 0;} on the list, but then i realize all the list become one giant none <br>
string, so i replace it with <div><p></p></div> cuz it is superior

5.) the footer is a problem, i can't find a way to put it exactly on the bottom of the container,
i tried {display: block;} cuz i thought maybe the deafult is inline, but no it didn't work, i don't know
the solution so i add {position: fixed;}, a quick solution, but certainly not what i wanted,
i could increase the container sizes and put the footer inside, but all the parts inside the container had height and width
relative to the container (i used % instead of px), i don't want to remake all the sizes just to insert the footer.

### Built with

- no semantic, div is simpler for this one, at least for me, the only semantic is footer
- CSS
- flexbox, only used to make the container on the center with {justify-content: center;}
- no CSS Grid
- desktop-first workflow, breakpoint @400px
- no framework, cuz i still dont know how to used them

### What I learned

1.) alright so when i add @mediaquery, there was a time when the container was not on the center,
after i used flexbox and {justify-content: center;} it bugged out, i think it bugged out and it
became {justify-content: end;} by default

so what is did was insert {justify-content: start;} to test if the property worked,
fortunately it does work and i set it back again to center.

2.)the bottom margin is 0 by default, so i add {margin-bottom: ;}
i dont think it will work, but it did

### Useful resources

- [MDN web docs](https://developer.mozilla.org/en-US/) - I think everyone should know how to use this website, it is like wikipedia made only for coding
- [getcssscan](https://getcssscan.com/css-box-shadow-examples) - i used this website to copypaste the shadow style

## Author

- Frontend Mentor - [@ALtera21](https://www.frontendmentor.io/profile/ALtera21)
- github Profile - [ALTera21](https://github.com/ALtera21)
