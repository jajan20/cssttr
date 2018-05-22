## CSS to the Rescue
Link to  [Website](https://jajan20.github.io/cssttr/index.html)
![](https://raw.githubusercontent.com/jajan20/cssttr/master/preview.png)

## Table of Contents
- [Feedback](#feedback)
- [Week 1](#week-1)
    - [Progress](#progress)
    - [Review](#review)
    - [To do](#next-week)
- [Week 2](#week-2)
    - [Solution](#solution)
    - [Assignments week 2](#assignments-week-2)
    - [What is next](#what-is-next)
- [Week 3](#week-3)
    - [Assignments week 3](#assignments-week-3)
- [I learned](#i-learned)
- [Resources](#resources)


## Feedback

Below you'll find the biggest points I needed to change for my project. On the left things that had to be done and on the right how I fixed them. 

| To do's        | fixed how?                                                                                                                                             |
|----------------|--------------------------------------------------------------------------------------------------------------------------------------------------------|
| Rating system  | For the rating system I decided I wanted the emoticons to be the main input. Radio buttons are gone but still tab-able. Changed styling to horizontal. |
| Step indicator | This was a lot harder, figured out how to style progress bar.  Added grid to the navigation container.                                                 |
| Other fixes    | - Gave the main button elements a box-shadow instead of a border so that they don't jump anymore. - Changed styling.                                   |


## Week 1
#### Progress


- Sketched different layouts for a design.
- Used CSS Secrets to add different styles
    - [x] Fancy ampersands (page 462)
    - [x] De-emphasize by dimming (page 546)
    - [x] De-emphasize by blurring (page 555)
    - [x] Intrinsic sizing (page 602)
    - [x] Styling by sibling count (page 616)
    - [x] Vertical Centering (page 641)

While writing this I haven't used every style element mentioned above. Since I'm still changing my layout of the site. When I'll dive into styling my components I'm sure I can use the rest of the styling elements.

#### Review
I started off great, It's been a while since I worked with CSS. But as the code progressed I realized that writing CSS without the use of classes is quite the challenge. This resulted in a bit of spaghetti CSS, combining pseudo-classes to refer to the right element, using extra tags to fit my needs.

#### Next Week
###### To do
- [x] optimize the code
- [x] adding styling to the components
- [x] adding the "pleasureable"
- [x] Finish the assignment


## Week 2
This week, while working on the different components I realized my mistake. Instead of putting every HTML component into a single file, I used hrefs to link to new web pages. You may wonder why this would be a problem, so let me explain. 

Using pseudo-classes I can select different sections based on the hierarchy inside my document. But since my components all had their own file it got harder and harder to find ways to select the same (but different) elements.

#### Solution
So I killed my darling, threw everything away and started from scratch. This time every component is nested comfortably inside one file. But as you can see this also cost me a lot of time. But I'm pretty sure I can fix everything before the due date. 

#### Assignments week1
- [x] Loading spinner 8.43
- [x] Transitions on hover/focus 8.42
- [x] Cursor 6.29
- [x] Extending clickable area 6.30
- [x] Custom checkboxes 6.31
- [x] PSEUDO random background 2.7
- [x] Form validation 



#### What is next
- [x] Styling every component
- [x] Fixing CSS
- [x] Adding pleasurable user experience

## Sources
#### Attribute selector
[CSS Tricks](https://css-tricks.com/almanac/selectors/t/target/) for more info

Something that really helped me was discovering that we can select elements on their attribute(value?)

```css
[src*="boot"] {
  content: url("https://vasilis.nl/voto/fotos/klein/161001180558-de-boot-gemist-2500.jpg");
  width: 100%;
}
```
Although it's not really necessary in the example above it's still pretty cool. The img file didn't look really good. So I searched for the higher-res one. And by using the attribute value selector I made CSS look for an img where the source link contains the word boot. Very specific and this makes sure I'm only changing that image.

#### :target & visibility: visible;
[CSS Tricks](https://css-tricks.com/almanac/selectors/a/attribute/) for more info

Something else I thought was really cool. I wanted to make a pop-up window where the component would be displayed without using javascript. 

```css
section:target {
  visibility: visible;
  }
```
With help of [James P.P. Jefferies](https://github.com/Jamerrone) I could use # in my hrefs referring to these sections (only used for linking, **not for styling**). The section would be hidden first and with: target I could make them visible again and style them.

## Week 3

This was the last week for project CSS to the rescue, although it was quite the challenge I'm satisfied with the results. These last couple of weeks gave me a lot of headaches trying to find ways to select elements without using classes or ids. But with the things I've learned, I'm sure that in the future my designs will be a lot better and easier to use.

### Assignments week 3
At the end of week two, I made a to do for the upcoming week. It wasn't easy but I managed to tick off every checkbox.

- [x] optimize the code
- [x] adding styling to the components
- [x] adding the "pleasurable"


## I learned
##### Pseudo classes

- :target
- :nth-of-type
- :focus-within
- :first-letter
- :checked
- :after
- :valid

##### Properties
- outline-color:
- transition:
- content:
- align-self:
- visibility:

The list above contains the attributes/classes that surprised me the most. I had heard of them before, just never used them. For future projects, these will come in handy.

## Resources
- [CSS Tricks - Attribues](https://css-tricks.com/almanac/selectors/a/attribute/)
- [Grid by Example](https://gridbyexample.com/examples/ )
- [Example - Animation Ease](https://codepen.io/P1N2O/pen/pyBNzX)
- [Pseudo Classes](https://www.w3.org/TR/selectors-3/#the-user-action-pseudo-classes-hover-act)
- [CSS Grid Multiple Collumns](https://medium.com/@patrickbrosset/css-grid-css-multi-columns-7664f59bb60c)
- [HTML5 Forms](https://www.html5rocks.com/en/tutorials/forms/html5forms/)
