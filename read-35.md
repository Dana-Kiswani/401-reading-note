# *Pre-rendering and Data Fetching*

> By default, Next.js pre-renders every page. This means that Next.js generates HTML for each page in advance, instead of having it all done by client-side JavaScript. Pre-rendering can result in better performance and SEO.

> Each generated HTML is associated with minimal JavaScript code necessary for that page. When a page is loaded by the browser, its JavaScript code runs and makes the page fully interactive. (This process is called hydration.)


> *Note: You can also try the above steps on `localhost`, but CSS won’t be loaded if you disable JavaScript.*



# *Dynamic Routes*

> We can do this by taking the following steps. You don’t have to make these changes yet — we’ll do it all on the next page.

> First, we’ll create a page called [id].js under pages/posts. Pages that begin with [ and end with ] are dynamic routes in Next.js.

> In pages/posts/[id].js, we’ll write code that will render a post page — just like other pages we’ve created.


> The returned list is not just an array of strings — it must be an array of objects that look like the comment above. Each object must have the params key and contain an object with the id key (because we’re using [id] in the file name). Otherwise, getStaticPaths will fail.


# *Deploying Your `Next.js` App*

> If you’re NOT continuing from the previous lesson, you can download, install, and run the starter code for this lesson below. This sets up a nextjs-blog directory such that it’s identical to the result of the previous lesson.



> ***Before we deploy, let’s push our Next.js app to GitHub if you haven’t done so already. This will make deployment easier.***

> - *On your personal GitHub account, create a new repository called nextjs-blog.*
> - *The repository can be public or private. You do not need to initialize it with a README or other files.*
> - *If you need help setting up your repo, take a look at this guide on GitHub.*
