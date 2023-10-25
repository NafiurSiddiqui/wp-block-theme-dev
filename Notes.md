# Architecture

## Templates/

- `index.html` is the home of the block.
- Never put direct html inside the files inside this. will break and show and error on WP backend editor.
- Instead, everything needs to be `block`s there.

for example,the following is allowed but no direct `html elements`.

```
<!-- wp:paragraph -->
<p> A valid paragraph like this is allowed. </p>
<!-- /wp:paragraph -->

```

## Functions.php

- you will still need to register your custom blocks and so on.

# Hacks

- create your site with FSE and either copy paste from `flywheel -> open adminer -> select wp_posts -> select data -> last post` will have your saved structure. You can either copy or click the 3 dots on the top right corner from the post editor and look for export data. There you will have the post.

# Packages

- `@wordpress/script` : Is the golden one to have. Automatically manages manual setup for WP JS environment.
