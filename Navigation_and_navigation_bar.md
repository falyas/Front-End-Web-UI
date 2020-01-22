# Navigation and Navigation bar

## Why use website navigation?
* Most websites are not single pages
* Adds convenience
* Intuitive

## Information Architecture
* Structure of a system with respect to how information is organized and labeled
* Navigation methods provide access to Information
* Need to consider information architecture when designing a websites
* Need to consider information architecture when implementing a navigation pattern

## Website Hierarchy
* Typically a tree Structure
```
Home
│       
│
└───About
│   │   History
│   │   Mission
|   |   Key Players
│   │
│   └───Menu
│       │   Appetizers
│       │   Mains
│       │   Desserts
│   
└───Contact
    │   Technical Support
    │   Delivery Support
```

## Navigation Bars
* Expected at the top of the websites
* Contains links to website pages
* Design Dos
- Use simple, user-friendly terms
- Standardize Navigation
- Provide indication of user location within the webpage Hierarchy
- It's a standard convention to click on the logo to go to the home page
* Design Don'ts
- Too many options on the navigation Bar
- Generic and broad labels, ex: "Product", "Service"

## Breadcrumbs
* Another typical way to provide Navigation
* Typically near the top
* Secondary navigation, usually placed below the primary navigation and above the content
* Indicator of the current page's location within a navigational Hierarchy
- Path based: set of steps
- Location based: hierarchy toward the root
- Attribute based: set of choices

## Other navigation aids
* Tabs
* Pills
* Pagination
* dropdowns
*  Accordion
* Tags / Tag clouds
* Scrollspy
* Affix

## Sample Navigation Bar using Bootstrap 4

```HTML
<nav class="navbar navbar-dark navbar-expand-sm bg-primary-green fixed-top">
  <div class="container">
    <a class="navbar-brand" href="#">
      <ul class="navbar-nav mr-auto">
        <li class="nav-item">
          <a class="nav-link active" href="#">Home</a>
          <a class="nav-link" href="#">About</a>
          <a class="nav-link" href="#">Menu</a>
          <a class="nav-link" href="#">Contact</a>
        </li>
      </ul>
    </a>
  </div>
</nav>
```

"navbar-expand-sm" expands when the screen size is above the "sm" breaking-point. "mr-auto" specifies the right-margin. So, the content will be pushed as left as possible, within the navigation bar. "nav-item" allows navigation items to be displayed horizontally.

We can explicitly identify one of these links as active link, to tell the user that he/she are on that link. Use the "active" class to identify the current active link.
