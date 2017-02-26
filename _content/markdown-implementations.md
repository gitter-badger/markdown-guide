## Troubleshooting

### Discrepancies Between Implementations

Recall from a [previous section](#how-does-it-work) of this guide that an *implementation* takes Markdown-formatted text and outputs it to HTML format. In a way, an implementation is the realization of John Gruber’s Markdown design document as software — it uses Gruber's specifications to render your Markdown documents.

Unfortunately, since Gruber's documentation is somewhat vague on a variety of issues, many implementations interpret the Markdown syntax differently.  Discrepancies between implementations can result in unexpected variations when rendering Markdown.

In practical terms, this means that different Markdown applications will output the same Markdown-formatted text differently. If you copy and paste Markdown-formatted text from one Markdown application to another, the final output may look slightly different. This might seem like a minor issue, but it can cause big headaches down the road if you decide to migrate your Markdown documents to another application that uses a different implementation.

<div class="alert alert-info">
  <i class="fa fa-info-circle" aria-hidden="true"></i> <strong>Note:</strong> There are literally dozens of Markdown implementations available to developers. For a complete list, see <a href="https://github.com/markdown/markdown.github.com/wiki/Implementations">this wiki page on GitHub</a>. CommonMark maintains a list of <a href="https://github.com/jgm/CommonMark/wiki/List-of-CommonMark-Implementations">different implementations</a>.
</div>

#### Resolving Discrepancies

Discrepancies between implementations have frustrated Markdown users for years, and there's a good chance that you'll run into a discrepancy-related problem at some point in the future. Here are some suggestions for dealing with and resolving discrepancies:

- **Use best practices.** An old Greek proverb says that an ounce of prevention is better than a pound of cure. Since most discrepancies stem from uncommon or non-standard uses of Markdown, keeping your formatting simple and consistent will minimize your chances of encountering a discrepancy. You can use a Markdown linter to enforce best practices. The linter will proactively warn you when you do something wrong. There are many such tools available ([1](https://github.com/mivok/markdownlint), [2](https://github.com/DavidAnson/markdownlint),  [3](https://github.com/wooorm/remark-lint)) and there's also [a package for Atom](https://atom.io/packages/linter-markdown).
- **Read the docs.** Your first troubleshooting step should be to read your Markdown application's documentation and, if necessary, figure out which implementation your Markdown application is using. You might need to review the implementation's documentation to see how it interprets the Markdown syntax. For example, [Dillinger's](https://dillinger.io) documentation reveals that it uses the [markdown-it](https://github.com/markdown-it/markdown-it) implementation, which follows the CommonMark specification.
- **Stick with one implementation.** If at all possible, try to stick with the implementation you first used to output your Markdown-formatted text.
- **Investigate discrepancies.** You can use [Bablemark 2](http://johnmacfarlane.net/babelmark2) to compare the output of the various Markdown implementations. This web-based tool allows you to input Markdown-formatted text and see how it's rendered by virtually every Markdown implementation. The [FAQ for Bablemark 2](http://johnmacfarlane.net/babelmark2/faq.html) is also worth a look — it discusses many of the common discrepancies between implementations.

### Variant Lightweight Markup Languages

- CommonMark is a "a standard, unambiguous syntax specification for Markdown, along with a suite of comprehensive tests to validate Markdown implementations against this specification." There are now a number of implementations using CommonMark ([Dillinger](https://dillinger.io) uses one), and most of the applications
