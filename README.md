# cypress-playwright
> Run Cypress tests and Page Objects using Playwright

This package provides a bridge between Cypress and Playwright test runners. You can execute Cy tests using Pw.

---
Before using please read [this](https://cypresstips.substack.com/p/cypress-tips-april-2023) 🚨
---

## Beyond Joke

Despite the original implementation being an empty shell with no functionality,
it got 40+ GitHub stars, which is way more than whatever I (@jiridanek) ever published on GitHub myself.
This shows the motivating idea of the package is fairly sound,
and some kind of a product-market fit should be there to be found.

Cypress itself is aware of the gaps, and they were even working on Puppeteer integration,
to, for example, let you juggle those browser tabs (see below).

Anyway, this fork is a take on the original idea to make it work for a narrower use-case relevant to the fork owner.

### What's wrong with Cypress?

* https://docs.cypress.io/app/references/trade-offs
* some limitations may get resolved in time
  * https://github.com/cypress-io/cypress/issues/299
  * https://github.com/cypress-io/cypress/issues/30756

### What's wrong with Playwright?

Playwright (by default) does not use real browsers, it uses its own browser implementations.
* https://www.theautomatedtester.co.uk/blog/2023/the-login-test/

Playwright positioning is similar to Cypress: it's mainly a developer productivity tool and less of a QA testing tool.
Playwright is lot more QA department-friendly than Cypress, though.

## Install

```
# install this package using NPM
$ npm i -D cypress-playwright
# or using Yarn
$ yarn add -D cypress-playwright
```

If using Cypress, add this package to your [Cypress support file](https://on.cypress.io/support-file)

```js
// TODO
```

Voilá you can now run your Playwright tests in Cypress and Cypress tests in Playwright!
Plus use `await` keyword with all Cypress commands:

```js
// TODO
```

Want to open 2nd tab and test your chat application? No problem!

* [From the Founder: Cypress’ Evolution, Vision, and Roadmap | Brian Mann](https://www.youtube.com/watch?v=Br7mjzHIII0&t=929s) (at 13:18)
* https://github.com/cypress-io/cypress/blob/develop/npm/puppeteer/README.md

## Small print

Author: Gleb Bahmutov &lt;gleb.bahmutov@gmail.com&gt; &copy; 2023

- [@bahmutov](https://twitter.com/bahmutov)
- [glebbahmutov.com](https://glebbahmutov.com)
- [blog](https://glebbahmutov.com/blog)
- [videos](https://www.youtube.com/glebbahmutov)
- [presentations](https://slides.com/bahmutov)
- [cypress.tips](https://cypress.tips)
- [Cypress Tips & Tricks Newsletter](https://cypresstips.substack.com/)
- [my Cypress courses](https://cypress.tips/courses)

License: MIT - do anything with the code, but don't blame me if it does not work.

Support: if you find any problems with this module, email / tweet /
[open issue](https://github.com/bahmutov/cypress-playwright/issues) on Github

## MIT License

Copyright (c) 2023 Gleb Bahmutov &lt;gleb.bahmutov@gmail.com&gt;

Permission is hereby granted, free of charge, to any person
obtaining a copy of this software and associated documentation
files (the "Software"), to deal in the Software without
restriction, including without limitation the rights to use,
copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the
Software is furnished to do so, subject to the following
conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
OTHER DEALINGS IN THE SOFTWARE.

April 1st 2023
