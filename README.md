# Project Website for Q(AI)²
1. This repository is built on top of the
[Astro Framework](https://astro.build/)
2. ```Astro``` requires the ```npm``` ecosystem.
You will need to install ```Node.js```. See here: https://nodejs.org
3. After installing ```Node.js```, clone this repository and run the
following command to install the dependencies:
    ```sh
    npm install
    ```
4. Next, run the following command to start the development server
in your localhost environment.
The server should start listening on port 4321 (if default).
    ```sh
    npm run dev
    ```
4. To build to static assets, please run:
    ```sh
    npm run build
    ```


## Commands

All commands are run from the root of the project, from a terminal:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:4321`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |


## Project Structure

The project structure is the following.  
Currently, there are no fonts populated in the ```fonts``` folder.  
The PDFs folder holds the paper PDFs directly. If papers are linked instead, this folder can be deleted.  
Right now, there is one PDF checked into the git repository as it makes it easy to verify across instances.

```text
/
├── public/
├── src/
│   ├── assets/
│   │   └── fonts/
│   │   └── images/
│   │   └── PDFs
│   ├── components/
│   │   └── Card.astro
│   │   └── Footer.astro
│   ├── layouts/
│   │   └── Layout.astro
│   └── pages/
│       └── index.astro
│       └── impressum.astro
│       └── datenschutz.astro
└── package.json
```

Astro looks for `.astro` or `.md` files in the `src/pages/` directory. Each page is exposed as a route based on its file name.