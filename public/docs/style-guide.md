# Style Guide for Documentation

## About
Author: themathgenius

Last Updated: 31 July 2024

This will serve as the suggested template for all writeups and psr documentation (NOT including route notes) in this repository.
This won't be enforced, but having the same format for all documentation enables easier and more strategic reading.

## Format
Documents are expected to follow a certain output format.
* **Use markdown**, unless there's a specific reason to use another file type or format. Always include a file extension (.md, .txt, etc.).
  If you've never used markdown before, visit [markdownguide.org](https://www.markdownguide.org) to get started.
* **Include a title**. The title should be 10 words or less, or at least fit on one markdown line.
* **Include an "About" section**. See [above](#about) as an example. Include:
  * **Author**. SRC/Twitch/Discord usernames are all acceptable, as long as they are well-identifying.
  * **Last updated date** to identify potentially outdated/unfresh documents. Prefer \<day> \<month, written out> \<year>. 
  * **A brief introduction** to the document. Ideally a few sentences to overview what the document will cover.
* **Use headings to organize.** Use -- Section -- breakers for non-markdown files.
* **Use footnotes where necessary**. Markdown supports footnotes and convenient re-directs; use them where you can.
* **Content should make sense standalone**.
  * Use discretion when determining the audience's prior knowledge.
    * For example, a FAQ should expect the reader to have little to no existing run knowledge,
      whereas a document/video outlining a new movement mechanic can expect the reader to have a basic to intermediate understanding of the speedrun.
  * Explain PSR-specific jargon and terminology, especially if it's niche.
  * The key exception to this rule is to link and reference other documents.
    * Links to external documents and other files in this repository are both okay, but please verify your links.
    * This will give readers the opportunity to learn more, while also avoiding the need to repeat yourself or others.

## File Naming
To keep links and file paths reasonably short, file names and paths are expected to follow a specific format.
* **Directories should be an abbreviated where possible**. This includes games, categories, etc. 
* **Keep filenames brief**. As a guideline, file names should be:
  * **lowercase alphanumeric words, hyphenated.**
    * Examples of accepted name formats:
      * hg-vs-ss-diff.md
      * text.md
      * 2024-07-30-log.md
    * Examples of names to avoid:
      * FRR2-notes.md (use of capital letters)
      * frr2_notes.md (use of underscores instead of hyphens to separate words)
      * shop@celadon.md (use of non-compliant character @)
      * frr2-notes (no file extension)
  * **As few words as possible**, as long as it is unique and descriptive within the context of its parent directory.
    * As an example, `frlg/glitchless/frlg-glitchless-faq.md` can be shortened to `frlg/glitchless/faq.md`.
      Since the file is already housed under `frlg/glitchless`, readers can infer a `faq.md` is for FRLG glitchless.
      But this should be explicitly stated in the About section (see "Contents should make sense standalone").

## Markdown code and other text guidelines
Raw text/code is expected to be spaced and organized to be readable and easily editable.
* There's no hard-set line limit, but **100 characters is the suggestion** for longer paragraphs.
  * Prefer line breaks between sentences or clauses.
