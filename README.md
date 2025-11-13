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

To add a new member, create a new subdirectory with their name under `content/authors/` and include the above-mentioned files.

The `_index.md` should include the following things:

```
title: [your name]
first_name: [your first name + middle name]
last_name: [your last name]
superuser: [false]
position: [int] (position of person "Meet the Group" list)
role: [name of subgroup you are a part of]
organizations:
  - name: [name of organizations/affiliations]
  - name: [There may be multiple organizations/affiliations]
website: [link to website]
interests:
  - [interest 1]
  - [interest 2]
  - [interest n]
social:
  - icon: [what icon fx. linkedin]
    icon_pack: [package that includes the icon fx. fab]
    link: [link to social]
email: [enter email to display Gravatar (if Gravatar enabled in Config)]
highlight_name: [highlight the author in author lists? (true/false)]
user_groups:
  - [name of subgroup you are a part of]
```

### Managing Publications

New publications are automatically processed using **GitHub Actions**. To add a new publication:

1. Add the BibTeX entry for your latest publication to `publications.bib`.
2. Submit a **Pull Request** with the updated `publications.bib` file.
3. Once merged, GitHub Actions will generate a new directory under [`content/publication`](content/publication).
