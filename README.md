# The Lab for Neuroimaging and Neuroinformatics (LNN) @ UCPH

This is the official website for the Lab for Neuroimaging and Neuroinformatics (LNN) at the University of Copenhagen (UCPH). Below are instructions for configuring and updating the site.

## Configuration

Most of the configuration is managed in the [`config/_default`](config/_default) directory.

- The **baseURL and title** are defined in `hugo.yaml`.
- The **navigation bar** is specified in `menu.yaml`.
- The **weight parameter** determines the order in which links appear in the navigation bar.

For more details on configuring Hugo, refer to the [Hugo documentation](https://gohugo.io/documentation/).

## How to Add Content

### Updating the Main Page
The main page content is stored in [`content/_index.md`](content/_index.md) and is structured in blocks. You can modify this file to update the homepage text or layout.

For advanced customization, refer to the [Hugo documentation on content organization](https://gohugo.io/content-management/organization/).

### Adding Lab Members
Lab members are listed in the [`content/authors`](content/authors) directory. Each member has their own folder containing:
- An `_index.md` file with their profile details.
- An `avatar.jpg` for their profile picture.

To add a new member, create a new subdirectory with their name under `content/authors/` and include these two files.

### Managing Publications
New publications are automatically processed using **GitHub Actions**. To add a new publication:
1. Add the BibTeX entry for your latest publication to `publications.bib`.
2. Submit a **Pull Request** with the updated `publications.bib` file.
3. Once merged, GitHub Actions will generate a new directory under [`content/publication`](content/publication).

