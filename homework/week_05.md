---
title: "Week 05"
---

a)  **What is Quarto?**
Quarto is open-source scientific and technical publishing system that we can use to create reproducible presentations and materials. 

b)  **How do you make columns using Revealjs in Quarto Presentations?**

We can make columns using .columns and adjust their width using the width attribute:

:::: {.columns}

::: {.column width="40%"}
Left column
:::

::: {.column width="60%"}
Right column
:::

::::


c)  **How would you change the appearance of slides using Revealjs in Quarto Presentations?**

There are many settings that we can use to change the appearance of slides using Revealjs. These are some background formatting options:

To add a background image: background-image. 
To change the size of the image: background-size (cover is the default size). 
To move the image:  background-position (default is center).
To repeat the background: background-repeat (default is no repeat). 
To change the opacity of the image: background-opacity (on a scale between 0 (transparent) and 1 (fully opaque)). 

We can also make use of the theme feature of Revealjs to set a theme for the presentation (set to moon below). 

---
title: "Presentation"
format:
  revealjs: 
    theme: moon
---

d)  **What has been the biggest constraint working on your own research project in the past week?**
I'm not sure if this is a constraint necessarily, but it was hard/frustrating to work through errors. Some errors take me a while to work through and it can be frustrating that it makes the process goes so slowly.

Also, as you know, I make a lot of mistakes in my code. While I usually get an error message, I worry that there are some that might go undetected and mess up my analysis. Not sure how common that is, though. 