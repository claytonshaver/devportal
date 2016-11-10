# devportal <sub><sup>| Cloud Elements developer portal</sup></sub>

This site is powered by [Jekyll](http://jekyllrb.com/), with a [Twitter Bootstrap Theme](http://themes.getbootstrap.com/products/dashboard) added.

The master branch is continuously deployed to production.

_Please_, feel free to make any contributions you feel will make Cloud Elements Documentation better.

**Submit all pull requests to the master branch**

## Installation

```bash
$ git clone git@github.com:cloud-elements/devportal.git
$ cd devportal
$ sudo gem install jekyll redcarpet jekyll-sitemap
```

## Usage

```bash
$ jekyll serve
```

Now browse to [http://127.0.0.1:4000/](http://127.0.0.1:4000/) and code away!

## Site Structure

Element Docs will be placed in their respective folder, e.g. Salesforce.
The Element Docs are structured in the following way:

```bash
|-- root
  |-- docs
    |-- elements
      |-- element folder (e.g. Salesforce)
        |-- element specific docs (e.g. endpoint setup, create instance)
```

Platform docs like Hub level documentation, Events Framework, and OAuth Proxy are located at the `docs -- platform` level:

```bash
|-- root
  |-- docs
    |-- platform
      |-- event-management
        |-- event-management specific docs (e.g. how to guides, videos)
```

Product docs like Element Builder, Mapper, Groud2Cloud, Formulas are located at the `docs -- products` level:

```bash
|-- root
  |-- docs
    |-- products
      |-- element-builder
        |-- element-builder specific docs (e.g. how to guides, videos)
```

Quick Start docs like authentication and FAQs are located at the `docs -- getstarted` level:

```bash
|-- root
  |-- docs
    |-- getstarted
      |-- authentication
```

## Conventions

All documents are composed in markdown.  HTML can be used right in the markdown docs.

### Pages

You can write pages in markdown, HTML, or HAML. They all get converted to HTML when the site is generated.

The site uses the Redcarpet Markdown Syntax
[View Cheatsheet](https://caleorourke.gitbooks.io/redcarpet-syntax/content/cheatsheet/index.html)

Pages have a block of YAML at the top that sets a few options. They are pretty self explanatory; here's an example of an Element YAML:

```
---
heading: Salesforce CRM
seo: Overview | Salesforce CRM | Cloud Elements API Docs
title: Overview
description: Integrate Salesforce CRM into your application via the Cloud Elements APIs.
layout: docs
breadcrumbs: /docs/elements.html
elementId: 23
parent: Back to Element Guides
order: 1
sitemap: false
---
```

here's an example of a Product YAML:

```
---
heading: Instance APIs
seo: Instance APIs Overview | Cloud Elements API Docs
title: Overview
description: Find API documentation and example API calls.
layout: docs
platform: instances
breadcrumbs: /docs/platform/platform-docs.html
parent: Back to Platform Docs
order: 1
sitemap: false
---
```

## License
(The MIT License)

Copyright © 2012-2016 Cloud Elements Inc [http://cloud-elements.com/](http://cloud-elements.com/).

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the ‘Software’), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED ‘AS IS’, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
