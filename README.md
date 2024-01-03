# Personal Portfolio Project

Welcome to my project creating a personal portfolio, demonstrating my personality and progression as a junior full stack software developer. This was created using HTML and SCSS (Sass).

## Table of Contents

1. [Overview](#overview)
2. [HTML Structure](#html-structure)
3. [SCSS Structure](#scss-structure)
4. [About Me](#about-me)

## Overview

My portfolio is divided in sections to display relevant information about myself for potential employers, colleagues and members of the tech community.

- **Header**: Displays my name and navigation bar which can shortcut which section the user would like to view.
- **Intro**: Displays name, job title and image. 
- **About Me**: Displays an image of myself and information about my journey in addition to aspects of my personality.
- **Technical Skills**: Displays the coding languages and skills I have obtained.
- **Projects**: A grid displaying projects I have currently completed including the coding language and a screenshot. The repository and live site are also linked for viewing.
- **Footer**: Access to my GitHub, Linkedin and CV. 

## HTML Structure

The HTML is split into a header, main and footer. Within the main section, there are sections which are divided depending on the information stored.

## SCSS Structure

### Responsive Design
The profile is responsive depending on the device screen size with the use of media queries.

```
@media screen and (min-width: 768px) {
    .header {
        /stylings for the specific screen size/
    }
}
```

### CSS Grid
The Technical Skills and Projects sections layout were created using CSS Grid.

```
&__grid {
        display: grid;
        justify-items: center;
        align-items: center;
        padding: 20px;
        gap: 35px;
        grid-template-areas:
            'spring-boot java react'
            'bem scss javascript'
            'css3 html5 git';

        &--item1 {
            grid-area: git;
        }

        &--item2 {
            grid-area: html5;
        }

        &--item3 {
            grid-area: css3;
        }

        &--item4 {
            grid-area: javascript;
        }

        &--item5 {
            grid-area: scss;
        }

        &--item6 {
            grid-area: bem;
        }

        &--item7 {
            grid-area: react;
        }

        &--item8 {
            grid-area: java;
        }

        &--item9 {
            grid-area: spring-boot;
        }
    }
```

### CSS Flexbox

In 768px, the introduction is laid out using CSS flexbox.

```
&__words {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: flex-end;

        }
```
