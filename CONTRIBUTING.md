<!--suppress HtmlDeprecatedAttribute -->
<img align="center" alt="banner contributing" src="/.github/assets/GophigureBannerContributing.svg">

---

<h4 align="center"><i>A document containing information and guidelines applied-as-default to
Gophigure's projects.</i></h4>

---

<p align="center"><i>First off, thank you for taking the time to contribute to Gophigure! We greatly appreciate it. 🎉</i></p>

The following sections contain information and guidelines about how you can contribute to Gophigure
and its projects.

> 🔔 **Note:** Found an issue with this document? Consider opening an issue
[here](https://github.com/Gophigure/.github/issues/new) or creating a
> pull-request to address it [here](https://github.com/Gophigure/.github/pulls).

---

### Table of Contents

- [I Just Want to Ask a Question!](#i-just-want-to-ask-a-question)
  <br/>
  > ---
- [What Should I Know Before I Start?](#what-should-i-know-before-i-start)

    - [What is Gophigure?](#what-is-gophigure)
    - [Our Projects](#our-projects)
    - [The Go Programming Language](#the-go-programming-language)
    - [Design Decisions](#design-decisions)
      <br/><br/>
  > ---
- [How Can I Contribute?](#how-can-i-contribute)

    - [Reporting Bugs & Security Issues](#reporting-bugs--security-issues)
    - [How do I Submit a Bug or Security Issue?](#how-do-i-submit-a-bug-report-or-security-issue)
    - [Suggesting Features](#suggesting-features)
    - [How do I Submit a Feature Request?](#how-do-i-submit-a-feature-request)
    - [Code Contribution](#code-contribution)
    - [How do I Contribute Code?](#how-do-i-contribute-code)
    - [Pull-Requests](#pull-requests)
      <br/><br/>
  >   ---
- [Style Guide](#style-guides)

    - [Commit Messages](#commit-messages)
    - [Go Style Guide](#go-style-guide)
    - [Documentation Style Guide](#documentation-style-guide)

---

### I Just Want to Ask a Question!

If you'd like to ask questions about our projects, your best bet is to use GitHub's "Discussions"
feature for the related repository. Don't forget to check if your question **has been answered
before**.

We also have a [Support Server](https://discord.gg/7jPSgv5x76). Please visit the `#support` channel
to ask for help!

<h4 align="right"><i>
Don't ask to ask! — <a href="https://dontasktoask.com/">See why</a>.
</i></h4>

---

### What Should I Know Before I Start?

#### What is Gophigure?

Gophigure is an organization for projects revolving around our Discord bot, under the same name. We
aim to provide code that not only benefits *our* bot, but the projects of many others, not even
necessarily other Discord bots!

#### Our Projects

|                      Project                      |        Language(s)         | Description                                                                                                                           |
|:-------------------------------------------------:|:--------------------------:|:--------------------------------------------------------------------------------------------------------------------------------------|
|      [bot](https://github.com/Gophigure/bot)      |            `Go`            | The bot is our Discord bot, which uses the Gophigure name. It aims to provide quick & easy tools for Discord servers, as well as fun! |
|    [glyde](https://github.com/Gophigure/glyde)    |            `Go`            | Glyde is our Discord API wrapper used in our bot project, but is free to use for others!                                              |
|  [website](https://github.com/Gophigure/website)  | `JavaScript`, `TypeScript` | This is the website code for Gophigure and its projects.                                                                              |
| [branding](https://github.com/Gophigure/branding) |           `N/A`            | This project holds assets for our branding.                                                                                           |

#### The Go Programming Language

Most of our code is written using `Go`, and it is expected that you know the basics before
contributing to our code.

If you don't know much about `Go` and would like to know more, you can do so at
[the website](https://go.dev/).

#### Design Decisions

Normally, each of our projects has a clear and concise idea of its direction, and how it's going to
reach its destination.

In the event a project does *not* have a direction or clear destination, or you're unsure of either,
this doesn't mean you cannot contribute. Continue as normal, making your changes and submit the
pull-request. Your code will most likely be reviewed, and if we find anything out-of-place, we'll
let you know.

---

### How Can I Contribute?

#### Reporting Bugs & Security Issues

This section guides you through submitting reports of bugs or security issues in our projects.

> 🔔 **Note:** When submitting an issue, you need to consider the following:
> - Your report must be **easy to understand**.
> - You must include instructions on how to **reproduce** the behaviour.
> - Use **keywords** in your issue title.

Before submitting an issue, check
if [it already exists](https://github.com/Gophigure/bot/labels/bug). If it does, and it's still
open, consider commenting on it that you are also experiencing the issue (do __NOT__ open a new
issue), with the related information as mentioned in the notes above.

#### How do I Submit a Bug Report or Security Issue?

Bugs and security issues are tracked using GitHub issues for the related repository. If a template
for a repository is provided for submitting reports, please use it as it makes maintainer's lives
easier.

> 🔔 **Note:** If you notice any issues with our template(s), don't hesitate to
> shoot us a pull-request fixing the issue, we'll likely be more than happy to
> merge!

If your report is about performance, make sure to evaluate the perceived performance loss and make a
judgement on whether it is **currently important**. We want to hear your reasoning as to why we
should improve the performance, as doing this subtracts time from developing new features and
improving existing ones. Don't be upset if we mark these kinds of reports as `won't fix` or imply
that we will not take time to fix the problem immediately.

If you're using our projects with 3rd-party modifications, ensure that the issues still occur in our
unmodified projects. Issues brought on by additions or changes to our software is likely not a fault
of our own, however if you think that it is, don't hesitate to still make a report.

Don't forget to **include details** such as:

- Operating System
    - Name (Windows, MacOS/OSX, Linux, BSD)
    - Version/Distribution (11, Monterey, Ubuntu 22.04, FreeBSD 13.0)  
      *We may request more information about the specific build of your OS, such as the kernel or
      build number.*
    - Bit-ness (32 or 64 bit)
- Central Processing Unit (CPU)

  > 🔔 **Note:** Not all CPU details are **required**, just enough to get a rough idea of its
  performance and architecture.

    - Company
    - Brand
    - Family/Brand Modifier
    - Generation
    - Performance Level
    - Model/SKU Number
    - Power/Product Line Suffix
    - Architecture

  e.g `AMD Ryzen 5 3600X` or `Intel Core i7 8750H`

#### Suggesting Features

This portion gives you some pointers for submitting requests for features to be added to our
projects.

> 🔔 **Note:** When submitting a request, you need to consider the following:
> - Your request must be **easy to understand**.
> - You must **give reasons** for why you think the feature should be included.
> - Use **keywords** in your issue title.

Before submitting a request, check if
[it already exists](https://github.com/Gophigure/bot/labels/feature%20request). If it does, and it's
still open, consider commenting on it if you have something to add.

#### How do I Submit a Feature Request?

Feature requests are tracked using GitHub issues for the related repository. If a template is
provided for feature requests, please use it as it makes maintainer's lives easier.

> 🔔 **Note:** If you notice any issues with our template(s), don't hesitate to
> shoot us a pull-request fixing the issue, we'll likely be more than happy to
> merge!

If your request is for something outside the project's scope, don't be upset if we close the issue
with a statement giving this as a reason. Projects usually have a clear idea of the direction they
want to take, and this means mostly ignoring ideas that do not fit within those ideals. If you still
think you have a strong argument for the feature, don't be afraid to still submit a request.

#### Code Contribution

Contributing code to our projects is greatly appreciated, but of course we have a process that you
must follow to make it both easier for you, and easier for the maintainers.

Issues and pull-requests have labels which help to identify the area, severity, or potential
complexity of a possible solution.

#### Issue Tag Examples

> 🔔 **Note:** Some tags will only appear on **closed** issues, and if you're
> looking to contribute, they may not matter.

|                    Tag                     | Description                                                                                           |
|:------------------------------------------:|:------------------------------------------------------------------------------------------------------|
|                   `bug`                    | The issue is reporting incorrect behaviour.                                                           |
|             `good first issue`             | The issue is recommended for new contributors to tackle.                                              |
|              `documentation`               | The issue is related to adding or improving documentation.                                            |
|             `feature request`              | The issue is requesting for a new feature to be added, or an existing feature to be improved/changed. |                                                            |

#### How do I Contribute Code?

You can contribute code by choosing a GitHub issue to address, then following the guide below.

#### Local Development

You can contribute to our projects' code with a few easy-to-use tools.

First off, some programs you **require**:

- `git` — A version control system (VCS) tool, which you can
  obtain [here](https://git-scm.com/downloads).
- `git-lfs`* — Git Large-File-Storage (LFS) is an extension to `git` which allows versioning large
  and/or binary files.
- `go`** — The official Go programming language toolchain, which you can
  obtain [here](https://go.dev/dl).
- A text editor of your choice. This can be as simple as `notepad` or as complex as an Integrated
  Development Environment (IDE) like `Visual Studio Code`.***

> *Not all projects require `git-lfs`, but you may need it for some. If you
> would like to learn more about LFS you can do
> so [here](https://git-lfs.github.com/).

> **Not all projects require the Go toolchain, for example our website.

> ***In the event of using a text editor that supports the Language Server
> Protocol (LSP), you may want to install extensions and/or a language server
> for code-completion and other goodies to help development.

Once you've gotten the required tools to aid development, you can get started with the steps below.

1. Fork this repository, then clone your fork and `cd` into the folder.

    ```shell
    $ git clone <url> <folder-name>
    $ cd <folder-name>
    ```
   *Replace `owner` and `repo` with the name of the repository owner and the name of the repository,
   e.g. `Gophigure`and `bot`, to get `https://github.com/Gophigure/bot.git` & `bot_fork`.*
2. Create a new branch based of the existing branch you want to contribute to.

    ```shell
    $ git branch <new-branch-name>
    ```
   *If you do not have the correct branch checked out, instead use the name of the branch you want
   to duplicate as the first argument and the new branch name as the second. **
   e.g.** `dev feat/rewrite-x-system`
   or `dev fix/correct-type-for-x`.*
3. Make your changes and commit with them.

    ```shell
    $ git add <...files>
    $ git commit -m <commit-message>
    $ git push origin <branch-name>
    ```
4. Head back to GitHub and create the pull-request. If you need help creating pull-requests, check
   out [this](https://docs.github.com/en/github/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request)
   article written by GitHub themselves.

#### Pull-Requests

Pull-requests are an organised way to review contributions before merging.

When submitting pull-requests you **must**:

- Follow the [Style Guides](#style-guides).
- After you submit your pull-request, ensure
  all [status checks](https://help.github.com/articles/about-status-checks/)
  are passing.
- Respond thoughtfully to questions asked about your pull-request, whether it's from a maintainer or
  not.
    - You must be able to justify your changes.
    - You must be able to explain your changes.
- Try to make alterations when they are suggested or asked of you. This is often when we think your
  code doesn't quite fit our style, and we're just trying to keep things uniform.

<details>
  <summary><i>What if the status checks aren't passing?</i></summary>
  If your contribution isn't passing checks, and you believe that the failure
  isn't your own fault, please leave a comment on the pull request explaining
  why you believe it isn't related.
</details>

If you don't know how to submit a
pull-request, [this article](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request)
should help!

---

### Style Guides

#### Commit Messages

When writing a commit message, you **must** take these into consideration:

- Use present tense ("Add feature" and not "Added feature").
- Use imperative mood ("Move this to..." and not "Moves this to...").
- Limit the first line to 72 characters or fewer, but we won't hate you for not following this, and
  sometimes the maintainers forget this one too.
    - If you do happen to forget, maintainers might request that you alter the commit names to fit
      within 72 characters, or they will do it when merging.
- Prefix your commits with what action they perform and the scope, following
  the [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)
  guide.
    - e.g `feat(util): Add SomethingRather function` — You should not need to describe what your
      feature does, in most cases. Documentation along with the feature's name etc. should be
      enough.

#### Go Style Guide

Go formatting must *line up* with
the [Effective Go, Formatting](https://golang.org/doc/effective_go#formatting)
section in the Go documentation.

To save you reading most of it, `gofmt` will do most of the work for you. The Go toolchain
includes `gofmt` for you. Simply run it on any files you edit, some IDEs can be configured or come
pre-configured to run actions like these on-save.

Make sure to avoid platform-dependant code as best you can. If you require to use it, please make
justifications and ensure that all platforms are covered.

#### Documentation Style Guide

In-code documentation **must**:

- Follow the [Effective Go, Commentary](https://golang.org/doc/effective_go#commentary)
  section in the Go documentation.
- Ensure lines do not exceed 100 characters, any words that contain the 100 hard-limit within shall
  be placed on a new line. Punctuation may extend the 100-character limit, such as periods or
  commas, but not an apostrophe.
- Only use comment-blocks for comments that **require** it, please use line-comments for most
  documentation.
