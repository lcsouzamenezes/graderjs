<p align=center><img width=200 alt="Grader.JS logo image" src=https://github.com/c9fe/graderjs/raw/master/.readme-assets/grader_logo.png></p>

# [:goggles: GRaderJS](https://github.com/c9fe/graderjs) ![npm downloads](https://img.shields.io/npm/dt/graderjs?label=npm%20downloads) ![version](https://img.shields.io/npm/v/graderjs?label=version) [![visitors+++](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fc9fe%2Fgraderjs&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=%28today%2Ftotal%29%20visitors%2B%2B%2B%20since%20Nov%209%202020&edge_flat=false)](https://hits.seeyoufarm.com) 

Build cross-platform desktop apps without the bloat using JS, HTML and CSS.

## Details

Minimal binary is 10Mb (Windows, Hello World App). Typical Linux/MacOS binary is 14Mb (Hello World App).

<span id=top></span>
-------------------
- [Overview](##goggles-graderjs---)
  * [Details](#details)
  * [Advantages](#advantages)
  * [Disadvantages](#disadvantages-or-opportunities-and-opportunities-for-improvement-yes)
  * [Grader workflow](#grader-workflow)
  * [Extended Workflow](#extended-workflow)
  * [Ultimate Workflow](#ultimate-workflow-still-impossible)
  * [TOC](#toc)
  * [License](#license)
  * [Built with Grader](#built-with-grader)
- [Getting Started](#getting-started) 
  * [API & Documentation](#api-&-documentation)
  * [Extraordinary Control](#extraordinary-control)
  * [NodeJS related](#nodejs-related)
  * [App lifecycle](#app-lifecycle)
  * [Window related](#window-related)
  * [Docketty Docs](#docketty-docs)
  * [Questions](#questions)
- [Step by step guide](#step-by-step-guide)
  * [Get Started from the Command line](#get-started-from-the-command-line)
  * [Get Started from GitHub](#get-started-from-github)
  * [Start Building!](#start-building)
  * [Start Coding](#start-coding)
- [API](#api)
- [Then build it](#then-build-it)
- [Configuration](#configuration)
- [Screenshots](#screenshots)
- [More](#more)
- [Licensing](#licensing)
- [Related projects](#related-projects)
--------------------

## Advantages

- Simplicity. Grader is just a web server running on localhost viewed with the user's browser. If they have Chrome installed then you get a proper looking desktop app (thanks to the --app flag), and access to a bunch of cool APIs to control the browser (thanks to remote DevToosl protocol).
- Extensive APIs. Because you have access to Node.JS and, with Chrome, DevTools APIs there's so many things you can do. You can do almost anything.

<p align=right><a href=#top>Top</a></p>

## Disadvantages (...or, Opportunities, and Opportunities for Improvement? Yes)

- New. Undeveloped. Embryonic. Fragile. Untested. Unknown (relatively).
- Requires Chrome to be installed for a great experience (some people don't have it).
- Bundles Node.JS (and packs using upx but the binaries are still bigger than using Tauri or Neutralino).
- API still undeveloped and likely to change.
- Icons (for the binary) don't work (and it's a hard problem).

<p align=right><a href=#top>Top</a></p>

## Grader Workflow 

1. Create a new Grader app
2. Fill out the sections with your business logic and app specific node
3. Compile to get cross-platform binaries

<p align=right><a href=#top>Top</a></p>

## Extended Workflow 

4. Code-sign your binaries and upload them to app stores or GitHub releases or your own website.

<p align=right><a href=#top>Top</a></p>

## Ultimate Workflow (still impossible)

5. Use ~impossible non-existant~ ~(future?)~ packaging tool to bundle each binary in a soothing bath of platform specific app metadata that includes icons and associated weird OS specific coolness to make things truly awesome.

<p align=right><a href=#top>Top</a></p>

## License 

Copyright (c) 2020, Dosyago and/or its affiliates. All rights reserved.

This is a release of Grader, an cross-platform app builder.

License information can be found in the LICENSE file.

This software is dual-licensed. For information about commercial licensing, see [Dosyago Commercial License for OEMs, ISVs and VARs](https://github.com/dosyago/dual-licensing).

<p align=right><a href=#top>Top</a></p>

## Built with Grader

- [wingrader](https://github.com/c9fe/winrader) - windows 95 cross platform
- [jspaint.exe](https://github.com/c9fe/jspaint.exe) - classic paint cross platform

<p align=right><a href=#top>Top</a></p>

## Getting Started

```sh
npx graderjs my-app
```

<p align=right><a href=#top>Top</a></p>

### API & Documentation

Only a couple of API calls:

<p align=right><a href=#top>Top</a></p>

### Extraordinary Control

- constrol.send(command, params)
- control.on(eventName, handlerFunction) (also off)

*See commands available at [DevTools protocol homepage](https://chromedevtools.github.io/devtools-protocol/tot/)*

<p align=right><a href=#top>Top</a></p>

### NodeJS related

*As normal just use npm to add dependencies and import to use them*

### App Lifecycle

- launch: `go()` 
- shutdown: `stop()`

<p align=right><a href=#top>Top</a></p>

### Window Related

  - ui.open  
  - ui.close 
  - ui.move  
  - ui.size  
  - ui.minimize 
  - ui.maximize 
  - ui.restore  
  - ui.fullscreen  
  - ui.partscreen  
  - ui.getLayout
  - ui.openBlank (*not yet implemented*)
  - ui.writePage (*not yet implemented*)
  - ui.getScreen

<p align=right><a href=#top>Top</a></p>

### Docketty Docs

Then, read the [API docs](https://github.com/c9fe/grader-base/blob/master/README.md) or see below for the Getting Started Goose Guide.

<p align=right><a href=#top>Top</a></p>

### Questions

Open an issue!
  
<p align=right><a href=#top>Top</a></p>

## Step By Step Guide

### Get Started from Command line

Use npm to get the [Grader.JS tool](https://github.com/c9fe/graderjs) to automatically populate your new grader app.

```sh
  $ npm i -g graderjs@latest
  $ graderjs my-new-app
```

Then, read the [API docs](https://github.com/c9fe/grader-base/blob/master/README.md) or see below for the Getting Started Goose Guide.

<p align=right><a href=#top>Top</a></p>

### Or, get Started from GitHub

Click ["Use This Template"](https://github.com/c9fe/grader-base) on the base-repo and you will have a new repo, then clone it to your workspace and `cd` into it, and run:

```sh
npm i
```

<p align=right><a href=#top>Top</a></p>

### Start Building!

Read [the API docs](https://github.com/c9fe/grader-base), or create yer binaries right away:

```sh
./scripts/compile.sh
```

You now have a GUI app in Node.JS and JavaScript/HTML/CSS.

And you will have cross-platform binaries available in `/bin`

(*and also for download from the computer you're on at port 8080.*)

<p align=right><a href=#top>Top</a></p>

### Start Coding

Put your own code into, `src/app.js`:

**E.g**:

```js
  import Grader from './index.js';

  start();

  async function start() {
    await Grader.go();
  }
```

And put your JS/HTML/CSS into, `src/public/index.html`:

```html
  <meta charset=utf-8>
  <title>Your Cross-Platform App</title>
  <style>
    :root {
      font-family: sans-serif;
      background: lavenderblush;
    }
    body {
      display: table;
      margin: 0 auto;
      background: silver;
      padding: 0.5em;
      box-shadow: 0 1px 1px purple;
    }
    h1 {
      margin: 0;
    }
    h2 {
      margin-top: 0;
    }
  </style>
  <h1>Hello World!</h1>
  <h2>Meet <i>Grader</i></h2>
  <p>
    <button onclick="grader.ui.minimize();">_</button>
    <button onclick="grader.ui.restore();">&#11036;</button>
    <button onclick="grader.ui.close();">x</button>
  <script>
      (async () => {
        await graderReady();

        const [title, favicon, startURL] = (await Promise.allSettled([
          grader.meta.getTitle(),
          grader.meta.getFavicon(),
          grader.meta.getStartURL()
        ])).map(({status, value, reason}) => {
          if ( status == 'fulfilled' ) return value;
          return reason;
        });

        console.log({title, favicon, startURL});

        document.title = title;
      })();
    </script>
```

### API

Read [the API docs](https://github.com/c9fe/grader-base)!

<p align=right><a href=#top>Top</a></p>

### Build it

```sh
./scripts/compile.sh
```

You now have a GUI app in Node.JS and JavaScript/HTML/CSS.

And you will have cross-platform binaries available in `/bin`

and also for download from the computer you're on at port 8080.

For more demos see the demos in `src/demos`.

### Configuration

You can configure some options, via the configuration located in `src/config.js`:

```js
module.exports = {
  name: "MyGraderApp",
  entry: "./app.js",
  author: {
    name: "my name",
    url: "https://github.com/my-github-username",
  },
  desiredPort: 49666,
  version: "0.0.1",
  description: "A Beautiful Demonstration",
  source: "https://github.com/my-github-username/MyGraderApp",
  organization: {
    name: "My Org",
    url: "https://github.com/my-github-org-name"
  },
  apiOrigins: [],      // origins allowed to call API from UI (not implemented)
  DEBUG: false         // switch on debug output when you're ready to debug
}
```

<p align=right><a href=#top>Top</a></p>

## Screenshots

![Windows Grader](https://github.com/c9fe/graderjs/raw/master/.readme-assets/wingrader.JPG)
![Linux Grader](https://github.com/c9fe/graderjs/raw/master/.readme-assets/grader.JPG)

<p align=right><a href=#top>Top</a></p>

## More

See [the API docs](https://github.com/c9fe/grader-base) for more. Or just read the README.md of the grader app you've just created, it contains the full API docs. You can also take a look at the API code in `src/index.js`.

<p align=right><a href=#top>Top</a></p>

## Licensing

You're free to use this so long as you abide by AGPL-3.0. If you want to use it commercially or don't want this license, you can [purchase an exemption](mailto:cris@dosycorp.com?subject=Grader.JS).

<p align=right><a href=#top>Top</a></p>

## Related projects

See [this list of Electron alternatives](https://github.com/sudhakar3697/electron-alternatives) for more options for cross-platform desktop app developement using web technologies.

<p align=right><a href=#top>Top</a></p>

----------------------

# *Grader.JS!*
