## Troubleshooting



### General Tips

It's frustrating when Markdown-formatted text doesn't render the way you expect it to. If you notice something unusual happening, try these quick tips to fix it:

- **Double check your syntax.** Make sure you haven't fat-fingered something. Are you sure you used the right formatting? 
- **Try something else.** There are many different ways to do things in Markdown. Have you tried adjusting the formatting of the problem area? Remember that you can also use HTML tags in Markdown files.
- **Ask for help.**
- **Switch to a different application.**


### Discrepancies Between Processors

Recall from a [previous section](#how-does-it-work) of this guide that a Markdown processor takes Markdown-formatted text and outputs it to HTML format. In a way, a processor is the realization of John Gruber’s Markdown design document as software — it uses Gruber's specifications to render your Markdown documents.

Unfortunately, Gruber's documentation is somewhat vague on a variety of issues, so many processors interpret the Markdown syntax differently. Discrepancies between processors can result in unexpected variations when rendering Markdown.

In practical terms, this means that different Markdown applications output the same Markdown-formatted text differently. If you copy and paste Markdown-formatted text from one Markdown application to another, the final output may look slightly different. This might seem like a minor issue, but it can cause big headaches down the road if you decide to migrate your Markdown documents to another application that uses a different processor.

<div class="alert alert-info">
  <i class="fa fa-info-circle" aria-hidden="true"></i> <strong>Note:</strong> There are <a href="https://github.com/markdown/markdown.github.com/wiki/Implementations">dozens of Markdown processors</a> available to developers. CommonMark maintains a list of <a href="https://github.com/jgm/CommonMark/wiki/List-of-CommonMark-Implementations">different processors</a>.
</div>

#### Resolving Discrepancies

If you encounter a discrepancy, use these suggestions to resolve it:

- **Use best practices.** An old Greek proverb says that an ounce of prevention is better than a pound of cure. Since most discrepancies stem from uncommon or non-standard uses of Markdown, keeping your formatting simple and consistent will minimize your chances of encountering a discrepancy. You can use a Markdown linter to enforce best practices. The linter will proactively warn you when you do something wrong. There are [many](https://github.com/mivok/markdownlint) [such](https://github.com/DavidAnson/markdownlint) [tools](https://github.com/wooorm/remark-lint) available, and there's also [a package for Atom](https://atom.io/packages/linter-markdown).
- **Read the docs.** Your first troubleshooting step should be to read your Markdown application's documentation and, if necessary, figure out which Markdown processor your application is using. You might need to review the processor's documentation to see how it interprets the Markdown syntax. For example, [Dillinger's](https://dillinger.io) documentation reveals that it uses the [markdown-it](https://github.com/markdown-it/markdown-it) processor, which follows the CommonMark specification.
- **Stick with one processor.** If at all possible, try to stick with the processor you first used to output your Markdown-formatted text.
- **Investigate discrepancies.** You can use [Bablemark 2](http://johnmacfarlane.net/babelmark2) to compare the output of the various Markdown processor. This web-based tool allows you to input Markdown-formatted text and see how it's rendered by virtually every Markdown processor. The [FAQ for Bablemark 2](http://johnmacfarlane.net/babelmark2/faq.html) is also worth a look — it discusses many of the common discrepancies between processors.