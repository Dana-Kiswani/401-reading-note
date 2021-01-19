# *Assets, Metadata, and CSS*


> `Next.js` has built-in support for `CSS` and `Sass`. For this course, we will use `CSS`.

> *This lesson will also talk about how Next.js handles static assets like images and page metadata like the `<title>` tag.*


***Download Starter Code (Optional)***

> *If you’re NOT continuing from the previous lesson, you can download, install, and run the starter code for this lesson below. This sets up a nextjs-blog directory such that it’s identical to the result of the previous lesson.*


> *Again, this is NOT necessary if you’ve just finished the previous lesson.*

``` ruby
npx create-next-app nextjs-blog --use-npm --example "https://github.com/vercel/next-learn-starter/tree/master/assets-metadata-css-starter"
```
  
  
***Assets***

> *First, let’s talk about how Next.js handles static assets such as images.*

> *Next.js can serve static files, like images, under the top-level public directory. Files inside `public` can be referenced from the root of the application similar to `pages`.*

``` ruby
<img src="/vercel.svg" alt="Vercel Logo" className="logo" />
```

> *The logo image exists inside the public directory at the top level of your application.*


<hr>


***Metadata***

> `<title>` is part of the <head> HTML tag, so let's dive into how we can modify the <head> tag in a Next.js page.

*Open pages/index.js in your editor and find the following lines:*

``` ruby
<Head>
  <title>Create Next App</title>
  <link rel="icon" href="/favicon.ico" />
</Head>
```

> *Notice that `<Head>` is used instead of the lowercase <head>. <Head> is a React Component that is built into Next.js. It allows you to modify the <head> of a page.*
  
***NOTE***

> *To learn more about the Head component, check out the API reference for next/head.*

> *If you want to customize the `<html>` tag, for example to add the lang attribute, you can do so by creating a `pages/_document.js` file. Learn more in the custom Document documentation.*
