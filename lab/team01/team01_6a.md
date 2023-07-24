---
layout: default
title: team01-6a
description: "Adding the fixture"
layout: default
parent: team01
grand_parent: lab
---

# {{ page.title}} - {{page.description}}

The model to follow here is [`frontend/src/fixtures/restaurantFixtures.js`](https://github.com/ucsb-cs156-s23/STARTER-team01/blob/main/frontend/src/fixtures/restaurantFixtures.js)

The purpose of the fixtures file is to serve as a source of examples objects.  It has several use cases:
* "A single source of truth" to document the fields that you are expecting in an object of this type.
* A source of example data for the Storybook stories
* A source of data to be used in tests

The fixtures files are one of the few cases where we implement code, but don't also implement a test to go along with it.

To create your fixtures file, create a file with a similar name, e.g.
* `hotelFixtures.js`
* `bandFixtures.js`
* `bookFixtures.js`
* etc...

First, lets understand the code inside `restaurantFixtures.js`:

Inside the file, at the top level, we see this (with some code omitted so we can focus on the big picture):

```javascript
const restaurantFixtures = {
   // code omittted  
};

export { restaurantFixtures };
```

This sets the variable `restaurantFixtures` to a Javascript object (delimited by a set of curly braces, `{ }`), and then exports that variable so that 
you can import the variable in another file with code like this (from [`RestaurantForm.stories.js`](https://github.com/ucsb-cs156-s23/STARTER-team01/blob/main/frontend/src/stories/components/Restaurants/RestaurantForm.stories.js)

```
import { restaurantFixtures } from 'fixtures/restaurantFixtures';
```

Diving a bit deeper into the `restaurantFixtures` object, but still omitting some detail, we see that the
structure of the object is a set of key/value pairs.  The two keys in this case are `oneRestaurant` and `threeRestaurants`.
In each case, the values are arrays (delimited in Javascript by a set of square brackets, `[ ]`).  Keys are followed by a colon (':')
and then the value.  Key/value pairs are separated by commas. 

```js
const restaurantFixtures = {
    oneRestaurant:
    [
      // details omitted
    ],

    threeRestaurants:
    [
      // details omitted
    ]
};
```

Finally, we can look inside `oneRestaurant` and see that the value of `oneRestaurant` is an array containing a single object
representing the fields in a restaurant:

```js
oneRestaurant:
    [
      {
       "id": 1,
        "name": "The Habit",
        "address": "888 Embarcadero del Norte",
        "city": "Isla Vista",
        "state": "CA",
        "zip": "93117",
        "description": "Burgers and Fries"      
      }
    ],
```

Note that in the current starter code `STARTER-team01`, our implementation only provides for `id`, `name`, and `description`.  The intent is to eventually implement the fields `address`, `city`, `state`, and `zip` as well.  For the fixtures you create, it is only necessary to put in fields for `id` and the three fields you intend to implement as part of your CRUD operations.

The value of `threeRestaurants` is similar, so we won't describe it in detail, but look it over before continuing to make sure you understand the code.

Now, you are ready to create a fixtures file for your object.  For the instructions, we'll assume that you are creating fixtures for a hotel;
adjust the instructions accordingly for your object.

1. Start with a copy of `restaurantFixtures.js`
2. Do a search/replace on `restaurant`, replacing it with `hotel` (or whatever).
3. Replace the object inside what was `oneRestaurant` but is now, for example, `oneHotel`, with one that has the key/value pairs of the fields you
   want for your object.  Keep the `id` field (which should be an integer), but replace the other fields of `restaurant` with key/value pairs
   that are appropriate for your object.  You need a minimum of three fields beyond `id`; you can implement more if you like, 
   but since this is just an exercise, I suggest you keep it simple.
4. Now replace the objects inside `threeHotels` with three objects that are different from (and have different id values) from the ones
   in your `oneHotel` object.  I suggest that you keep the sample ids as `2`, `3`, `4`, since that will make coding the tests later 
   easier&mdash;the example tests expect the id of one of the fixtures to be `2`, `3` and `4`.  But it's your choice. Just know that if you
   choose different id numbers, you'll need to adjust the testing code later accordingly.
5. When your new `hotelFixtures.js` file (for example) is done, commit the change, and do a pull request. 

   For your PR title, use something like `Add fixtures for hotel objects`.
   
   Normally a PR description might need to contain screenshots, or testing instructions, but in this case, it can be
   very simple.  I suggest something like this:

   ```
   In this PR, we add fixtures for hotel objects to be used in testing and storybook entries.
   ```
6. When you've made the PR, drag the issue on the Kanban board into `In Review`.
7. Then, assign yourself a new issue from `ToDo`, and drag that into the `In progress` column, and start work on that issue.


