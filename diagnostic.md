# Ember Routing Diagnostic

Record your responses inside the fenced code blocks below each question.

1.  What are the main task(s) you perform inside the Ember Application Router,
    and what are the main task(s) you perform inside an Ember Route?

    ```md
  The main task you perform in the Router is defining and linking all the routes to
  the app. An ember route is linked to a template
    ```

1.  What is the command to generate a route named `boston` nested under
    `campus`?

    ```md
  ember generate route campus/boston
    ```

1.  Suppose you have a nested route at the URL `/campus/boston`. How would you
    use the `link-to` helper to generate an appropriate link?

    ```md
{{#link-to 'campus.boston'}}Campus{{/link-to}}
    ```

1.  Explain **at least** two differences between the following two route
    definitions.

    ```js
    this.route('products', function () {
      this.route('product', { path: '/:product_id' }); // <= 👀here
    });

    this.route('product', { path: '/products/:product_id' }); // <= 👀 here
    ```

    ```md
The 1st one makes the path to product_id a function while the other one does not.
You can make the guess that there are two product_id files. One within the app folder
and another within the products folder.
    ```

1.  Suppose we have the following route definition:

    ```js
    this.route('movie', { path: '/movies/:movie_id' }); // <= 👀 here
    ```

    If we navigate in the browser to `/movies/123`, how can we reference the
    value `'123'` inside a Route?

    ```md
    <!-- your response here -->
    ```

1.  Inside a template, how do we reference data provided by a Route?

    ```md
    We call it inside the template using a model. It directs us back to the
    model function from the Route.
    ```
