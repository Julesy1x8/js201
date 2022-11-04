# Coding Nomads JavaScript 201 Labs

**Important** first steps to get set up:

Do _not_ fork!

1. **Clone** this repository to your machine.
2. Create a _new_ repository on your GitHub account. _Don't_ fork this repository. Don't clone it yet. Take note of the URL of your new, blank GitHub repository:

   ```text
   git@github.com:<YOUR_USERNAME>/<YOUR_REPOSITORY_NAME>.git
   ```

3. From the command line, navigate to your local clone of _this_ repository and view the remote:

   ```bash
   $ git remote -v
   origin git@github.com:CodingNomads/js_201_labs.git (fetch)
   origin git@github.com:CodingNomads/js_201_labs.git (push)
   ```

   This should show you the URL of the Coding Nomads js_201_labs repository as above. You'll be changing this to your new empty repository:

   ```bash
   $ git remote set-url origin git@github.com:<YOUR_USERNAME>/<YOUR_REPOSITORY_NAME>.git
   ```

   Then run `git remote -v` to check that it's been replaced.

   Finally, you are ready to push the labs to your blank repository:

   ```bash
   git push
   ```

   This will update your blank repository with all the commits done on the labs repository.

4. Create a branch to work on, and once you are ready for your mentor to look over your work, create a pull request and request a review from them. Then you'll merge it together. Start new branches and pull requests for each section.

If at any point you are stuck or are unsure, reach out to your mentor, or post in the forum.

## How to Go Through These Labs

You'll see the course structure mirrored in the `labs` folder. At the end of each corresponding chapter, you should do the labs in the folder.

Some folders don't have any labs, usually because that chapter was focused on building the module project.

Throughout the course there are "Spoilers" and excercises for you to do. Place the results of those excercises in the corresponding folders in your repository so that your tutor can look over your work.

### Present Your Solutions

For many of the excercises, you'll need to create corresponding HTML files so that the solutions can be loaded in a live server.

For example, say one of the chapter folders had three files:

```text

00_SAMPLE
├ 01 - exercises
│ ├ process data.md
│ ├ create table.md
│ └ special methods.md
│
...

```

You will generally only need to create one sandbox per chapter:

```diff

  00_SAMPLE
  ├ 01 - exercises
  │ ├ process data.md
  │ ├ create table.md
  │ ├ special methods.md
+ │ └ solutions
+ │   ├ solutions.html
+ │   └ script.js
  │
  ...

```

Though in some cases, you may be asked to create more sandboxes, and along with the sandbox you may need to complete the "spoiler" exercises, you could end up with many sandboxes per chapter:

```diff

  00_SAMPLE
  ├ 01 - exercises
  │ ├ process data.md
+ │ ├ process data
+ │ │ ├ process_data.html
+ │ │ └ script.js
  │ ├ create table.md
+ │ ├ create table
+ │ │ ├ create_table.html
+ │ │ └ script.js
  │ ├ special methods.md
+ │ ├ special methods
+ │ │ ├ special_methods.html
+ │ │ └ script.js
+ │ ├ mini project
+ │ │ ├ mini_project.html
+ │ │ └ script.js
+ │ └ chapter excercises
+ │   ├ chapter_excercises.html
+ │   └ script.js
  |
  ...

```

You will be told when you need to break out into new sandboxes. By default, you should start a `solutions` sandbox in each chapter.

If you have a few, keep things organized by keeping an `index.html` file at the top level with links to all your sandboxes:

```diff

  00_SAMPLE
  ├ 01 - exercises
+ | ├ index.html
  │ ├ process data.md
  │ ├ process data
  │ │ ├ index.html
  │ │ └ script.js
  │ ├ create table.md
  │ ├ create table
  │ │ ├ index.html
  │ │ └ script.js
  │ ├ special methods.md
  │ ├ special methods
  │ │ ├ index.html
  │ │ └ script.js
  │ ├ mini project
  │ │ ├ index.html
  │ │ └ script.js
  │ └ chapter exercises
  │   ├ index.html
  │   └ script.js
  |
  ...

```

The top level index file can then be populated with links, the `href` attribute can point to the folder, if the folder has a `index.html` file:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <!-- ... -->
  </head>

  <body>
    <a href="process data">Process Data</a>
    <a href="create table">Create Table</a>
    <a href="special methods">Special Methods</a>
    <a href="mini project">Mini Project</a>
    <a href="chapter exercises">Chapter Exercises</a>
  </body>
</html>
```

Within each sandbox, you can optionally use the HTML to present the results of the labs, along with the console outputs.
