# CodeyOverflow Forum

In this project, we will build the beginnings of a web forum! A forum is an online discussion board where users can exchange their opinions on a variety of topics. The most important component of a forum is the comment section. This is what we’ll work on in this project.

In building this application, you will sharpen your skills in React components by practicing using props as well as defining, rendering, and referencing components.

# Tasks

**Setting Up Header and Body**

**1.** Take a look at the files provided for this project.

There is a file named `commentData.js` which contains an array of comment objects with `profileImg`, `username`, and comment as its properties. You will use this to populate the comments on the forum.

Your comment section will be composed of Card components, which will be comprised of smaller Header and Body child components.

Next, `App.js` will contain the top-level component. The data in `commentData.js` will be retrieved in `App.js` and flow downward from `App` to `Card` to `Header` and `Body`.

`index.js` will render the App component. style.css and index.html handle the markup and styling of the forum.

Once you feel comfortable with the structure of this application, move on to the next Task.

**2.** Let’s start with the smallest component, the Body. The Body is responsible for showing the comments that users have written. It will work with the comment property of our passed-down comments object extracted from commentData.js.

Open up `Body.js` and define your Body component.

This component should receive props. This props object contains all of the data on our comment, such as the username, profile image, and comment, but the Body works specifically with only the comment property.

Have the component return a `<p>` element that contains the comment property from props.

**3.**
Export the Body component after its function definition so that it can be imported and used in `Card.js`.

**4.** Open `Header.js` and define your `Header` component.

This component will be responsible for the profileImg and username properties of our passed-down comments object.

The Header component should receive props. The component should return two elements, an `<img>` element whose src attribute will receive the profileImg property from props, and a `<h1>` element, displaying username from `props`.

**5.**
Export the `Header` component after its function definition so that it can be imported and used in `Card.js`.

**Setting Up Card**
