`````markdown
## General Do's and Don'ts for Open-Source READMEs

- **Do use a clear, descriptive title and tagline.** Start with `# ProjectName` and a one-sentence summary. For example:
  _Good:_ `# goodice – A minimal TTRPG dice library in Go.`
  _Bad:_ Vague or missing titles.

- **Do write in the first/second person, present tense, active voice.** Speak directly to the reader in an informal but respectful tone. Use "we/our" and "you" where appropriate. For example: _"ProjectName is a lightweight platform… You can use it either as a complete backend…"_
  _Don't_ use passive voice or third-person ("the user can…"). Avoid overly formal or detached language.

- **Do keep paragraphs short (3–5 sentences) and break content into sections.** Use `##` and `###` headings to organize content — for example: **About**, **Installation**, **Usage**, **Configuration**, **Contributing**, **License**.
  _Don't_ bury important information in dense paragraphs.

- **Do provide example code blocks and command snippets.** Use fenced code (triple backticks) with a language hint where possible (e.g. ` ```go ` or ` ```yaml `).
  _Don't_ inline code without formatting; avoid ambiguous formatting that makes commands hard to copy.

- **Do use lists for clarity.** Use `-` or `*` for bullet lists of features or options, and numbers for step-by-step instructions.
  _Don't_ create bulleted lists with inconsistent punctuation. Avoid capitalizing mid-sentence after a comma (e.g. `* X is an optional integer, How many dice to roll.`); instead, make each bullet a complete sentence or clause.

- **Do cite or link resources and related projects.** Provide links to documentation, websites, or sibling projects.
  _Don't_ omit URLs for key resources. Ensure all links are complete and working.

- **Do include badges and images thoughtfully.** Use relevant status badges (license, build status, version) at the top. Use emojis sparingly for emphasis (e.g. ⚠️ for a preview warning).
  _Don't_ clutter the title with unrelated emoji or badge text.

- **Do explicitly list license and contribution guidelines.** Add a `## License` section with the license name and a link. Add a brief `## Contributing` section encouraging pull requests and linking to any templates or code of conduct.
  _Don't_ leave readers guessing the license or contribution process.

- **Do maintain a consistent voice and formatting.** Use present tense ("This library _provides_ X") and consistent spelling and grammar. Proofread for capitalization, typos, and punctuation consistency.

- **Do show installation steps.** Include a `go get`, build command, or Docker command early in the README, along with any required environment variables or prerequisites.
  _Don't_ assume users know how to install; be explicit about port numbers, dependencies, and setup steps.

- **Do outline the contribution flow.** Provide a simple checklist or flowchart (using Mermaid or similar) guiding new contributors: fork → clone → branch → code → test → PR → review. This clarifies expectations and etiquette.

- **Don't include irrelevant details or off-topic jokes.** Humorous asides (e.g. "I think you know what an integer is") are not necessary. Keep the focus on instructive content.

## Before/After Examples

Selected excerpts with revised versions following these recommendations.

- **Heading Levels:** Don't use `#` mid-document for sub-sections.
  - _Before:_

    ```markdown
    # Run a demo

    > assumes a terminal opened within the cloned repository...
    ```

  - _After:_

    ```markdown
    ## Run a demo

    > _Assumes a terminal opened within the cloned repository..._
    ```

    _Change:_ Use `##` instead of `#` for sub-section headings; italicize or rephrase side notes.

- **Voice and Clarity:** Avoid slang and parenthetical asides.
  - _Before:_
    ```markdown
    A constant is an integer number (e.g. `7` or `42` - I think you know what an integer is)
    ```
  - _After:_
    ```markdown
    A constant is an integer (for example, `7` or `42`).
    ```
    _Change:_ Remove casual remarks; keep it concise.

- **Complete Sentences in Bullets:** Maintain consistent punctuation.
  - _Before:_
    ```markdown
    - X is an optional integer, How many dice to roll. If not provided, 1 die is assumed.
    - d simply is "d" or "D"
    ```
  - _After:_
    ```markdown
    - **X** is an optional integer (how many dice to roll). Defaults to 1 if omitted.
    - **d** stands for "die" (the literal 'd' character).
    ```
    _Change:_ Bold the variable name, use correct punctuation, and write complete sentences.

- **Code Block Fencing:** Use fenced blocks for multi-line code.
  - _Before:_
    ```markdown
        blog_name: Blog
        site_url: http://localhost:8080 # the URL...
    ```
  - _After:_
    ````markdown
    ```yaml
    blog_name: Blog
    site_url: http://localhost:8080 # the URL...
    ```
    ````
    _Change:_ Add explicit fences with a language hint.

- **Grammar and Typos:** Fix wordiness and formatting of code references.
  - _Before:_
    ```markdown
    If you are going to use a script many times, it will be more efficient to reuse a Goodice instance.
    ```
  - _After:_
    ```markdown
    If you will use a script repeatedly, reuse a `Goodice` instance for better efficiency.
    ```
    _Change:_ Simplify phrasing and format inline code names correctly.

---
`````
