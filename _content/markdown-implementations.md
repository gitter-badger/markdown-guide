## Troubleshooting

### Discrepancies Between Implementations

You might recall from a [previous section](#how-does-it-work) of this guide that an implementation takes Markdown-formatted text and outputs it to HTML format. An implementation is the realization of John Gruber’s Markdown design document as software.

Unfortunately, since Gruber's documentation is somewhat vague on a variety of issues, many implementations interpret the Markdown syntax differently. The discrepancies between implementations can result in unexpected rendering of Markdown.

In practical terms, this means that different Markdown applications will output the same Markdown-formatted text differently. If you copy and paste Markdown-formatted text from one Markdown application to another, the final output may look slightly different.

You can use [Bablemark 2](http://johnmacfarlane.net/babelmark2) to compare the output of the various Markdown implementations. This web-based tool allows you to enter Markdown-formatted text and see how it's rendered by virtually every Markdown implementation. The [FAQ for Bablemark 2](http://johnmacfarlane.net/babelmark2/faq.html) is also worth a look — it discusses many of the common discrepancies between implementations.

<div class="alert alert-info">
  <i class="fa fa-info-circle" aria-hidden="true"></i> <strong>Note:</strong> There are literally dozens of Markdown implementations available to developers. For a complete list, see <a href="https://github.com/markdown/markdown.github.com/wiki/Implementations">this wiki page on GitHub</a>. CommonMark has <a href="https://github.com/jgm/CommonMark/wiki/List-of-CommonMark-Implementations">different implementations</a>.
</div>

### Other Lightweight Markup Languages
