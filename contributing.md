We'd love it if you could help make the Hacktoberfest Swag List even better. That's the spirit of open source after all!

Check Issues and current Pull Requests before contributing to avoid adding duplicates.

Adding a new company to the list
Please follow these rules regarding how to add a new company to the List:

Rules of Contributing
If you wish to add something to the Hacktoberfest Swag List, that's great and we'd love to have you!

Please be sure to follow the simple rules:

Be sure you are looking to add something of substance to this project, not just spam PRs. PRs must meet the Hacktoberfest Quality Standards.
Verify that you have read the home page, and Readme.md on GitHub. You understand that this project is to connect maintainers with developers, not a way to get all the swag you can.
Please be available to make changes within 48 hours when requested to do so. If you don't, then your PR may be closed.
Please fix all issues flagged by the bots, including CodeClimate, GH Actions, Netlify, CircleCI or any others as soon as possible, ideally right away.
A company must have publicly posted about their swag. You should include a link back to the original blog post, tweet, GitHub issue, etc. where the swag can be verified.
If adding a new company to the swag list, follow the formatting below:
How to format your contribution
Make a fork of this repo and add the details for what company and swag you find in the list.md file located at /docs/list.md.

We are using a very simple language called Markdown to format this list. It's basically a way to make things look pretty without having to use a rich text editor. Please familiarize yourself with Markdown using this handy cheat sheet provided by GitHub (PDF).

New for 2022, we are only adding companies in an A->Z list and do not have a "Least Involvement to Most Involvement" section anymore. Why? Because this repo isn't about doing the least amount of effort to get a sticker or socks, it's about connecting you to companies who go above and beyond for Hacktoberfest. Thus, only an alphabetical list will be maintained this year.

A to Z Order of Companies
Find the first letter of your company within the list, then add your information in the correct alphabetical order by using the following Markdown formatting:


#### **Company Name**

- **Swag**: (T-shirt, stickers, etc)
- **Requirements**: What do I have to complete? Are there different requirements per swag item? Are the PRs merged or just submitted?
    - Indented lists require a Tab or 4 spaces instead of 2 spaces due to MkDocs formatting weirdness.
- **How to sign up**: Link to signup page using inline formatting of [text](URL)
- **Issues**: Optional link to Hacktoberfest tagged issues.
- **Notes**: If needed, otherwise write "N/A". This is where links to blog posts/tweets go.
If you don't see a letter heading for your company, please add it! Use the Markdown formatting to do so:


### A
Setting up the site locally
You will need following dependencies already installed in your system to set up MkDocs locally:

Python 3.8
pipenv
Setting up the repository
To get the site up and running locally, follow the below steps:

Fork the repository here.

Create a local clone of the website:


git clone git@github.com:<YOUR-USERNAME>/hacktoberfest-swag-list.git
Change into the hacktoberfest-swag-list directory:

cd hacktoberfest-swag-list
Run MkDocs
Install the required dependencies

pipenv install
Build the site and make it available on your local server for live viewing:

mkdocs serve
Please make sure you are always making changes in the Markdown docs located in /docs/ and do not edit the HTML that MkDocs builds in the /site/ directory.

Setting up the site using Docker
Alternatively, you can use the native Mkdocs-Material Docker imgage to build this site locally. The Dockerfile found here pulls in the Mkdocs-Material Docker image and adds the markdown-link-attr-modifier plugin so that the links continue to open in new tabs without having to add the tags manually.

Build the latest version of this image:


docker build -t squidfunk/mkdocs-material .
Run the Docker instance:


docker run --rm -it -p 8000:8000 -v ${PWD}:/docs squidfunk/mkdocs-material
Other Contributing Guidelines
Issues are not assigned to any one person. Please don't ask for an Issue to be assigned to you. All meaningful PRs will be reviewed first-come-first-served due to Hacktoberfest only being a month long.
Disclaimer: This website is a fan and community made creation. It is not affiliated with Hacktoberfest or any company offering swag.

Presented by DigitalOcean

If you're looking for the Swag List from 2018 through 2021 click here for the GitHub releases, click here for the tags, and see the 2018, 2019, 2020, and 2021 branches.
