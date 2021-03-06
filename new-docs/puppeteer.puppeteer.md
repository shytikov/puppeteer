<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [puppeteer](./puppeteer.md) &gt; [Puppeteer](./puppeteer.puppeteer.md)

## Puppeteer class

The main Puppeteer class. Provides the [launch](./puppeteer.puppeteer.launch.md) method to launch a browser.

When you `require` or `import` the Puppeteer npm package you get back an instance of this class.

<b>Signature:</b>

```typescript
export declare class Puppeteer 
```

## Remarks

The constructor for this class is marked as internal. Third-party code should not call the constructor directly or create subclasses that extend the `Puppeteer` class.

## Example

The following is a typical example of using Puppeteer to drive automation:

```js
const puppeteer = require('puppeteer');

(async () => {
  const browser = await puppeteer.launch();
  const page = await browser.newPage();
  await page.goto('https://www.google.com');
  // other actions...
  await browser.close();
})();

```
Once you have created a `page` you have access to a large API to interact with the page, navigate, or find certain elements in that page. The [\`page\` documentation](./puppeteer.page.md) lists all the available methods.

## Properties

|  Property | Modifiers | Type | Description |
|  --- | --- | --- | --- |
|  [devices](./puppeteer.puppeteer.devices.md) |  | [DevicesMap](./puppeteer.devicesmap.md) |  |
|  [errors](./puppeteer.puppeteer.errors.md) |  | [PuppeteerErrors](./puppeteer.puppeteererrors.md) |  |
|  [product](./puppeteer.puppeteer.product.md) |  | string | The name of the browser that is under automation (<code>&quot;chrome&quot;</code> or <code>&quot;firefox&quot;</code>) |

## Methods

|  Method | Modifiers | Description |
|  --- | --- | --- |
|  [connect(options)](./puppeteer.puppeteer.connect.md) |  | This method attaches Puppeteer to an existing browser instance. |
|  [createBrowserFetcher(options)](./puppeteer.puppeteer.createbrowserfetcher.md) |  |  |
|  [defaultArgs(options)](./puppeteer.puppeteer.defaultargs.md) |  |  |
|  [executablePath()](./puppeteer.puppeteer.executablepath.md) |  |  |
|  [launch(options)](./puppeteer.puppeteer.launch.md) |  | Launches puppeteer and launches a browser instance with given arguments and options when specified. |

