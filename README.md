# Basic Docsify Github Template

This project is a basic template for creating a documentation site using [docsify](https://docsify.js.org/#/) and hosting it on [Github Pages](https://pages.github.com/). Docsify is a lightweight documentation framework that uses markdown files to generate a documentation site. It also has a rich community of plugins that can extend and customize the framework. Since sorting through all the plugins can be a bit overwhelming, this project has curated and integrated the most useful plugins to get you started.

## Getting Started

There are two methods for utilizing this repository as a template for your own documentation site. The first method is to use the Github template feature. This will create a new repository in your account that is a copy of this repository. This method is very convenient and well-suited for a standalone documentation repository.

The second method is to add this repository as a remote to your existing repository. This will allow you to pull in changes from this repository to a branch in your repository. This method allows you to keep your documentation in the same repository as your code. This method is well-suited for a documentation site that is part of a larger project.

### Template Adoption Method

Use this method if you are creating a standalone documentation repository.

1. Click the "Use this template" button at the top of the repository page.
2. Enter a name for your new repository.
3. Click the "Create repository from template" button.

Once created, you can clone your new repository and start editing the markdown files in the `docs` folder. You can also customize the site by editing the `index.html` file.

### Merge Adoption Method

Use this method if you want to add a documentation site to an existing repository.

1. Add this repository as a remote to your existing repository using the following command:

```bash
git remote add upstream-template git@github.com:tspauld98/basic-docsify-gh-template.git
```

2. Fetch the contents of the remote repository using the following command:

```bash
git fetch upstream-template
```

3. Create a branch to hold the contents of the remote repository using the following command:

```bash
git checkout -b upstream-template-main --track upstream-template/main
```

4. Switch back to the `main` branch using the following command:

```bash
git checkout main
```

5. Merge the contents of the `docs` directory from the remote repository into your existing repository's `main` branch using the following command:

```bash
git checkout upstream-template-main -- docs
```

6. Commit the changes to your repository using the following command:

```bash
git commit -am "Add docs folder from upstream-template"
```

**Note:** You make need to resolve any conflicts before you can commit the changes to the `main` branch.

Once you have the contents from the template repository in your existing repository, you can start editing the markdown files in the `docs` folder. You can also customize the site by editing the `index.html` file to make the site your own.

## Developing Your Documentation

### Prerequisites

Make sure the following software is installed on your system:

- [Node.js](https://nodejs.org/en/)
- [npm](https://www.npmjs.com/)
- [Docsify CLI](https://docsify.js.org/#/quickstart?id=quick-start)

### Development Process

This process assumes you have the prerequisites installed on your system and that you have used one of the methods above to create your documentation repository.  It also assumes that you have cloned the repository to your local system.

1. Make changes to the markdown files in the `docs` folder.  Mermaid and PlantUML are integrated with Docsify, so you can use them to create diagrams and illustrations in your documentation to support the text content.
2. Commit the changes to the local repository.
3. Run the following command to serve the documentation site locally:

```bash
docsify serve docs
```

4. Open a browser and navigate to `http://localhost:3000` to view the documentation site.
5. Repeat steps 1-4 until you are satisfied with the changes to the documentation site.
6. Push the changes to the remote repository on Github.

When you push the changes to the remote repository, Github will automatically deploy the documentation site to Github Pages if you have configured Github Pages for your repository. You can view the deployed site by navigating to `https://<your-github-username>.github.io/<your-repository-name>` once the Github deployment process has completed.

## Customizing Your Documentation Site

If you want to add or disable features, you will need to modify the `index.html` file.  The `index.html` file is the entry point for the documentation site.  It is a single page application that uses the markdown files in the `docs` folder to render the documentation site dynamically.  All the plugins currently configured have been included locally in the `_vendors` folder.  If you add plugins, you will need to add them to the `_vendors` folder and update the `index.html` file to include them or configure them to load them from a CDN.  The `_media` folder contains images and other media that are used in the documentation site.  You can add your own media to this folder including custom styles, custom Javascript code, images, videos, and audio files.

At a minimum, you should update the following items in the `index.html` file:

- Update the `title` tag in the `head` section of the `index.html` file.
- Update the `description` meta tag in the `head` section of the `index.html` file.
- Update the `shortcut icon` link tag in the `head` section of the `index.html` file and the `favicon.ico` file in the `_media` folder.
- Update the `name` attribute of the `docsify` script tag in the `body` section of the `index.html` file.
- Update the `repo` attribute of the `docsify` script tag in the `body` section of the `index.html` file.
- Update the `logo` attribute of the `docsify` script tag in the `body` section of the `index.html` file and the `logo*.png` file in the `_media` folder.
- Update the `name` attribute in the `autoFooter` attribute of the `docsify` script tag in the `body` section of the `index.html` file.
- Update the `url` attribute in the `autoFooter` attribute of the `docsify` script tag in the `body` section of the `index.html` file.
- Update the `copyYear` attribute in the `autoFooter` attribute of the `docsify` script tag in the `body` section of the `index.html` file.

Additionally, you should make any style changes in the `index.html` file to match the branding for your project/organization or to match your personal preferences.

## Deploying Your Documentation Site on Github Pages

TBD

## Dependencies and Plugins

TBD

## Future Enhancements

- [x] ~~Add a LICENSE file~~
- [x] ~~Add a robot.txt file~~
- [ ] Add a CONTRIBUTING file
- [ ] Add a CODE_OF_CONDUCT file
- [ ] Add a SECURITY file
- [ ] Add a CHANGELOG file
- [ ] Set up a .github folder
