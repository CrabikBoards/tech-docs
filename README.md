# Technical Documentation of Crabik boards

This repository contains the Technical documentation about Crabik products. It
can be viewed at https://tech-docs.crabikboards.com.

## Editing

There are two methods to view and edit the book. There is a quick method that
does not include additional UI elements such as search, and the complete way
that will render the book as it is rendered on the official website.

### GitHub (Quick)

The book can be viewed and edited on GitHub by going to
[src/README.md](src/README.md).

### mdBook (Complete)

- Install [mdBook](https://github.com/rust-lang/mdBook#installation)
- Install [mdbook-admonish](https://github.com/tommilligan/mdbook-admonish#installation)
- Install [mdbook-linkcheck](https://github.com/Michael-F-Bryan/mdbook-linkcheck#getting-started)
- Clone the repository using `git`.
- From the cloned repository, run `mdbook serve`
- You may now view the book at `http://localhost:3000`
- Edits are made in the `src` directory. The server will automatically update