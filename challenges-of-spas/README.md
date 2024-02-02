# ![Intro to SPAs - Challenges of SPAs](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will be able to discuss the challenges of Singele-Page Applications (SPAs)

## Challenges of SPAs

Let's dive into some of the challenges of Single-Page Applications (SPAs):

- **Search Engine Optimization (SEO) Concerns:** Search engines traditionally rely on HTML content to crawl and index web pages. SPAs dynamically load content using JavaScript, making it challenging for search engines to index the content effectively.

- **Initial Load Time:** SPAs often require a larger initial load time as all the necessary assets (HTML, CSS, JavaScript) are loaded at the beginning. This can lead to slower initial page rendering compared to traditional multi-page applications.

- **Complex State Management:** As a SPA grows, managing the application's state becomes more complex. With multiple components and views, ensuring that the application behaves as expected and maintaining a consistent state across the application becomes a tricker task.

- **Accessibility and Progressive Enhancement:** Some of a SPAs core features (dynamically updating content using JavaScript, URLs not updated server side, etc.) pose challenges in ensuring the application is accessible. There are also performance concerns, as SPAs are not always fast, particularly with slow network conditions.

## SEO Concerns

Imagine you are visiting a library in search of a specific book. You arrive and are looking for signs to direct you to the book's location, but there are no signs in sight. Your book is there, but you are definitely going to have a harder time finding it without the right indicators of where to look.

This illustrates the problems that SPAs encounter with search engines. Search engines like Google prefer websites where they can easily read and understand the content. In the case of a SPA, the dynamic loading of content using JavaScript might make it a bit more challenging for search engine (which traditionally rely on HTML) to follow and index all the details of the application and ahve it appear in search results.

## Initial Load Performance

SPAs often require a larger initial load time as all the necessary assets (HTML, CSS, JavaScript) are loaded at the beginning. 

The application needs to complete a number of tasks on page load, such as download large Javascript bundles that contain the application logic and dependencies, and fetch data and assets. The browser also needs to parse and execute the initial Javscript code. Depending on the size of the bundles and the amount of data being fetched, load times can be delayed.

You can compare this to loading up a backpack for a trip. Everything has to be packed from the start. Depending on how long the trip is, how many items you may need, or how many items you need to sort through, your packing time (think of this as your loading time) can take a bit longer.


## Complex State Management

Complex state management refers to handling our application's state (your application's data and information) effectively and efficiently as it grows.

Let's go back to our library example. The library (your application) holds many books (your application's state). The books are spread across various shelves, which represent the various parts of your application. Each shelf needs to communicate and share information with others.

Here are things to consider when managing this. These apply in the application's current state and as it grows. Here are a few:

* As more shelves are added, making sure they talk to each other and share the right information becomes tricky.
* Shelves might have smaller shelves nested inside. Managing information transfer and updating within this nested structure adds complexity.
* Figuring out how books (information) flow throughout the library without creating gaps and holes in shelves or other parts of the library is crucial. It's like making sure everyone in the library knows what's happening.
* Sometimes, information takes time to arrive, like ordering a book online. Manging the library while waiting for the orders to come in adds in another layer of complexity.


## Accessibility and Progressive Enhancement

Accessibility challenges within single-page applications (SPAs) revolve around the dynamic nature of SPAs and the asynchronous loading of content.  Here are some specific accessibility challenges, particularly with users who use assistive devices such as screen readers:

* SPAs don't trigger traditional page reloads when navigating between different views, making it difficult for screen readers to recognize and announce these changes. If the changes are recognized, they can be delayed.

* SPAs often have complex navigation structures with nested componenents (think of our nested bookshelves) and dynamically changing interfaces. If the screen readers have a hard time detecting the navigation structure and hierachy, it can be challenging for the users of screen readers to understand and naviagtion through the application. 

There are also some performance concerns with SPAs. Because SPAs load a substantial amount of Javasript at initial page load and often rely on asynchronous data retrieval through APIs, SPAs can be heavilty affected by poor network conditions. If networks are experiencing issues or do not have a strong signal, the application's performance will be slowed down or halted.
