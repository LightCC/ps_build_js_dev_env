# Testing Automation for JavaScript projects

## Testing Types

1. Unit
   1. This module only covers this
2. Integration testing between modules
3. UI (system) testing
   1. Selenium, etc.

## Testing Frameworks

1. Mocha
   1. Popular, Mature, a lot of support (we'll use this)
2. Jasmine
3. Tape
4. QUnit
5. AVA
6. Jest (Facebook)
   1. Just a wrapper over Jasmine

## Other Libraries

Assertion Libraries Provides the syntax and support for assertions

1. Chai
   1. We'll use this
2. Others - not really a bad option, just pick one

Helper Libaries

1. JSDOM
   1. Simulate the browser's DOM
   2. Run DOM-related tests without a browser
2. Cheerio
   1. jQuery for the server
   2. Query virtual DOM using jQuery selectors

## Where to run tests

1. Browser
   1. Karma
   2. Testem
2. Headless Browser
   1. PhantomJS
3. In-memory DOM
   1. JSDOM

## Where should I put my test files?

1. Centralized
   1. Less noise in src folder
   2. Deployment confusion?
   3. Inertia?
   4. (With Python Packages - allows only testing on final installed package...)
2. Decentralized
   1. No import problems
   2. Clear visibility
   3. Convenient to open
   4. No recreating folder structure
   5. Easy to move tests with the src file when refactoring

## When should tests run?

1. For Unit Tests - every time you hit save!
   1. Rapid feedback
   2. Facilitates TDD
   3. Automatic = Low friction!
   4. Increases test visibility
2. But... that will be too slow!!
   1. Unit tests should run fast (or you're doing it wrong!)
3. For Integration testing
   1. less often, they are slower
4. UI testing
   1. Before release
   2. Often includes clicking and waiting, etc.
