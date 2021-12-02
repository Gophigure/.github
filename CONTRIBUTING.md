# Contributing to Gophigure

To start, let's get something off our chest,

*Thank you for taking valuable time out of your day(s) and/or night(s) to contribute!!* 🎉

The following bullet-points and another tidbits are a set of guidelines and helpful information to get you started with
contributing to Gophigure, hosted [here](https://github.com/Gophigure/bot), as well as our other repositories on GitHub.
These are guidelines, they're not set-in-stone, and you're allowed to take some creative liberty and let use your best
judgement.

> **Note:** *Any qualms with this document? Open a [pull-request](https://github.com/Gophigure/.github/pulls) and correct something we missed, or something you think we could word better.*

## Table of Contents

- [I just want to ask a question!](#i-just-want-to-ask-a-question)


- [What should I know before I start?](#what-should-i-know-before-i-start)
    - [What is Gophigure?](#what-is-gophigure)
    - [The Go Programming Language](#the-go-programming-language)
    - [Gophigure Design Decisions](#gophigure-design-decisions)


- [How Can I Contribute?](#how-can-i-contribute)
    - [How Do I Submit a (Good) Bug or Security Concern?](#how-do-i-submit-a-good-bug-report-or-security-concern)
    - [Suggesting Features](#suggesting-features)
    - [How Do I Submit a (Good) Feature Request?](#how-do-i-submit-a-good-bug-report-or-security-concern)


- [Your First Code Contribution](#your-first-code-contribution)
    - [Local Development](#local-development)


- [Pull-Requests](#pull-requests)


- [Styleguide](#styleguide)
    - [Commit Messages](#commit-messages)
    - [Go Styleguide](#go-styleguide)
    - [Documentation Styleguide](#documentation-styleguide)


- [Additional Notes](#additional-notes)
    - [Issues and Pull-Request Labels](#issues-and-pull-request-labels)

## I Just Want to Ask a Question!

*"Don't ask to ask!"* - [See why](https://dontasktoask.com/).

> 🔔 **Note:** Do not create issues just to ask questions! Please use the resources below, not only does it make the maintainer's lives easier, but it also gets you faster responses.

We have an official [Support Server](https://discord.gg/7jPSgv5x76). Please visit the `#support` channel to ask for
help!

## What Should I Know Before I Start?

### What is Gophigure?

Gophigure is an open source project — it's comprised of not only the code, but the maintainers, contributors and those
who support the project. 🤖💓🧑

But, back to the code side of things, what *is* Gophigure? 🤔

- Gophigure is written solely using the Go programming language.
- Gophigure can be compiled into a single binary, only requiring a configuration file.
- As most Go libraries and programs are, Gophigure is split into multiple packages that group related code together,
  allowing the ability to keep certain code contained within a package and only allow global access to needed constants,
  variables, types or functions. ⚙️📦
    - `main` has code that allows easily setting up the full Gophigure bot, easily.
    - `core` comprises of code designed to be used **globally**, such as logging utilities or variables that relate to
      the core runtime.
    - `state` handles state-based stuff, that happens per-shard.
    - `extenions` contains structs that extend `arikawa`'s, providing more functionality.
    - `commands` contains the bot's commands.
    - `util` is made up of code that is designed to be helpful, such as string manipulation or matching any type of
      object within a slice!
        - `builders` is reserved for code designed for easily building complex or repeatable structs and data.

### The Go Programming Language

Gophigure is written using Go, it is required that you have at least *some* knowledge of the language. We don't consider
Gophigure to be a project where budding developers can use it as a testing grounds for submitting pull-requests that add
or change things for "the sake of learning," however this does not mean that we do not allow new developers to
participate in Gophigure's development. If you're new to Go, but want to provide genuine pull-requests, we're happy to
receive them, and we'll do our best to guide you. 🏃‍💨

### Gophigure Design Decisions

Gophigure is designed with the idea in mind that people will be able to easily expand upon it for their own needs, if
they choose to self-host it. While we provide limited support for issues that occur due to 3rd-party changes, we will (
eventually) provide guides to help those who wish to make Gophigure fit them and their server(s) better.

## How Can I Contribute?

### Reporting Bugs & Security Issues

This section guides you through submitting an issue regarding one or multiple bugs, as well as security issues.
Following these guidelines makes it much easier for maintainers and the community, as it gives them a standard and
easy-to-understand slice of information to digest. 🪲

> 🔔 **Note:** When submitting an issue, you need to consider the following:
> - Make sure your report is **easy to understand**. 📃🪶
> - Make sure you include instructions on how to **reproduce** the behaviour. 💻➡️💻
> - Make sure related posts are easier to find by using **keywords** in your issue title. *️⃣

> 🔔 **Note 2:** If you find a **closed** issue similar to yours, link it in the "Short Description" section.

Before submitting an issue, check if [it already exists](https://github.com/Gophigure/bot/labels/bug). If it does, and
it's still open, consider commenting on it that you are also experiencing the issue (do __NOT__ open a new issue), with
the related information as mentioned in the notes above.

### How Do I Submit a (Good) Bug Report or Security Concern?

Bugs and security issues are tracked using [GitHub Issues](https://github.com/Gophigure/bot/issues). After finding a bug
or security issue, fill out a report
using [the template](https://github.com/Gophigure/bot/blob/dev/.github/ISSUE_TEMPLATE/bug_report.yaml).

> 🔔 **Note:** If you notice any issues with our template(s), don't hesitate to shoot us a pull-request fixing the issue, we'll likely be more than happy to merge!

- **Use clear and concise titles.** This helps maintainers and the community easily identify the main concern of the
  issue without even having to click on it!
- **Describe the exact steps to take to reproduce.** Give as best detail as you can, this will help others reproduce and
  confirm your findings.
- **Provide specific examples when listing reproduction steps.** This will make it as clear as crystal 💎 to those who
  want to help by trying to reproduce. Why does it happen? When does it happen? Does it happen after a specific amount
  of time, or randomly?
- **Describe the incorrect behavior.** Why is it wrong? What does the bot do when the bug occurs?
- **Explain the behaviour you expected to see.** What behavior was expected of the bot, if it were to behave properly?
- **Include screenshots and animated GIFs of the bot malfunctioning for greater context.** It can sometimes help people
  if they have a visual representation of the issue occurring.
- **When reporting a "panic", include the stacktrace.** This helps developers identify the problem in where it occurs
  and how many layers it goes through.
- **If the problem is related to performance,** it'd be awesome if you could include a `pprof` heap, or even better,
  investigate it yourself and return with your findings. If you'd like to learn more about measuring performance in Go,
  check out [this article](https://golang.org/doc/diagnostics).

> 🔔 **Note:** When reporting issues, please ensure the problem persists in the OFFICIAL version of the bot, this only applies to those running their own modified versions of Gophigure.

Don't forget to **include details about your environment**, including the operating system, architecture, CPU, RAM (
speed and amount is enough), storage (amount is enough).

### Suggesting Features

This portion of the Contribution Guidelines guides you through submitting feature requests for Gophigure, including new
features and improvements or changes to existing ones. Following these guidelines makes it much easier for maintainers
and the community to understand your feature request(s) and find related requests 🔍.

Before submitting a request, check if [it already exists](https://github.com/Gophigure/bot/labels/feature%20request). If
it does, and it's still open, consider commenting on it if you have something to add.

### How Do I Submit a (Good) Feature Request?

> 🔔 **Note:** The information in this section refers specifically to our `bot` repository, however you can apply this knowledge to our other repositories, too, given proper adaptation.

Feature requests are tracked using [GitHub Issues](https://github.com/Gophigure/bot/issues). After coming up with a new
feature or addition to an existing one, fill out a request
using [the template](https://github.com/Gophigure/bot/blob/dev/.github/ISSUE_TEMPLATE/bug_report.yaml).

- **Use clear and concise titles.** This helps maintainers and the community easily identify the main idea of the
  request without even having to click on it!
- **Describe the exact ideas behind the request.** Give as best detail as you can, this will help others comprehend and
  give feedback.
- **Provide specific examples of what purpose a feature would serve.** This can make it easier for some people to
  understand *why* you are requesting something.
- **Include drafts or mockups.** It can sometimes help people if they have a visual representation of the feature, this
  of course isn't necessary at all, but it's still nice. 😀

## Your First Code Contribution

If you're unsure about where we need help with Gophigure, check out issues tagged with `beginner` and `help wanted`.

- [Beginner Issues](https://github.com/Gophigure/bot/labels/beginner) — Issues only requiring a small fix with limited
  testing, good for beginners!
- [Help Wanted Issues](https://github.com/Gophigure/bot/labels/help%20wanted) — Issues that could be more difficult to
  handle than `beginner` issues, and we're looking for help.

### Local Development

Gophigure can be developed locally using the `git` version control tool. We prefer the feature-branch approach to
contributing. .

1. Fork this repository, then clone your fork and `cd` into the folder.
    ```shell
    $ git clone https://github.com/owner/repo.git repo_fork
    $ cd repo_fork
    ```
   *Replace `owner` and `repo` with the name of the repository owner and the name of the repository, e.g. `Gophigure`
   and `bot`, to get `https://github.com/Gophigure/bot.git`.*
2. Create a new branch based of the existing `dev` branch.
    ```shell
    $ git branch new_branch_name
    ```
   *If you do not have the `dev` branch checked out, for whatever reason, instead use `dev` as the first argument and
   the new branch name as the second.*

   We prefer to use the feature branch technique for contributions that include new features, so you should name your
   branches `feat/<name>`, where `<name>` is the name of the feature. Submitting fixes or adding small, yet helpful
   features to existing ones does not require doing this.
3. Make your changes and commit with them.
    ```shell
    $ git add files
    $ git commit -m commit_message
    $ git push origin branch_name
    ```
4. Head back to GitHub and create the pull-request. If you need help creating pull-requests, check
   out [this](https://docs.github.com/en/github/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request)
   article written by GitHub themselves.

## Pull-Requests

What's described here has several purposes:

- Maintain the code quality of Gophigure
- Fix problems that are important to our users
- Allow for community engagement
- Allow easy review for contributors

If you'd like your contribution(s) to be accepted by the maintainers:

1. Follow the [styleguide](#styleguide).
2. After you submit your pull-request, ensure all [status checks](https://help.github.com/articles/about-status-checks/)
   are passing. <details><summary>What if the status checks aren't passing?</summary>If your contribution isn't passing
   checks, and you believe that the failure isn't related to your change(s), please leave a comment on the pull request
   explaining why you believe it isn't related. A maintainer will re-run the checks for you, and further conclusions
   will be made.</details>

This list isn't exhaustive, maintainers may ask for more information or extras to be completed before considering
merging your contribution(s). Maintainers will usually ask for this if you're making a big change or making a change
they don't immediately understand.

## Styleguide

### Commit Messages

- Use present tense ("Add feature" and not "Added feature")
- Use imperative mood ("Move this to..." and not "Moves this to...")
- Limit the first line to 72 characters or fewer, but we won't hate you for not following this, and sometimes the
  maintainers forget this one too.
    - If you do happen to forget, maintainers might request that you alter the commit names to fit within 72 characters,
      or they will do it when merging.
- Prefix your commits with what action they perform and the scope, following
  the [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) guide.
    - e.g `feat(util): add SomethingRather function` — You should not need to describe what your feature does, in most
      cases. Documentation along with the feature's name etc. should be enough.

### Go Styleguide

Go formatting must *line-up* with the [Effective Go, Formatting](https://golang.org/doc/effective_go#formatting) section
in the Go documentation.

To save you reading most of it, `gofmt` will do most of the work for you, and lucky for you, that comes with the `go`
binary when installing. Simply run `gofmt` on any files you edit.

But, some extra things we need to talk about:

- Avoid platform-dependant code
- Avoid lines of code that are much longer than 100 characters, consider using newlines and indenting.

### Documentation Styleguide

In-code documentation:

- Follow the [Effective Go, Commentary](https://golang.org/doc/effective_go#commentary) section in the Go documentation.
- Ensure lines do not exceed 80 characters, any words that contain the 80 hard-limit within shall be placed on a
  newline.
- Only use comment-blocks for comments that **require** it, please use line-comments for most documentation.

External documentation:

- TBA

## Additional Notes

### Issues and Pull-Request Labels

Labels make it trivial to search and filter issues and pull-requests, to let you look for what you are specifically
targeting, as well as sort in a variety of ways.

If you'd like to know more on how to search through issues, check
out [this article](https://help.github.com/articles/searching-issues/) by GitHub.

