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

5. Merge the contents of the remote repository into your existing repository using the following command:

```bash
git merge --allow-unrelated-histories upstream-template-main
```

## Developing Your Documentation Site

TBD

## Customizing Your Documentation Site

TBD

## Deploying Your Documentation Site on Github Pages

TBD

## Dependencies and Plugins

TBD

## Future Enhancements

- [ ] Add a LICENSE file
- [ ] Add a CONTRIBUTING file
- [ ] Add a CODE_OF_CONDUCT file
- [ ] Add a SECURITY file
- [ ] Add a CHANGELOG file
- [ ] Add a robot.txt file
- [ ] Set up a .github folder
