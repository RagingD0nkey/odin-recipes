# odin-recipes

In this [project](https://www.theodinproject.com/lessons/foundations-recipes) I will create a simple website showing a couple of recipes. 

## Goal
My main objective is to implement a simple design, allowing the user to go from one recipe to the other via a main index page.
However, I will present the website as a restaurant menu, linking all menu items to their own recipe. Even the cocktail !

Recipes will be linked to their original [page](https://www.allrecipes.com/) every time.

## Difficulties
1. Trying to create a navigation menu at the bottom of the page. Had to use non breaking space to mimic tab space `nbsp;`
2. Getting the following warning in HTML validation `Element ul not allowed as child of element ul in this context`. However, if I include the `<ul>` inside the `<li>` element, it adds a bullet point. Not sure how to go from there. **SOLVED!** I open the 1st level `<li>`, then `<ul>`,then all the other bullet points, and then close the 1st `<li>` like so :
```
{
<ul>
    <li>A
        <ul>
            <li>A1</li>
            <li>A2</li>
        </ul>
    </li>
</ul>
}
```

## Improvement
1. I would have liked to add a per/person ingredient list. If 2 peoples, halving ingredient, if 8, doubling it.