---
title: Features of Minimal Course
---

## Highlighting Texts & Hidden Links

|----------------------------------|--------------------------------|
| `**Important!**{:.important}`    | **Important!**{:.important}    |
| `**Highlight**{:.hl}`            | **Highlight**{:.hl}            |
| `[A hidden link](URL){:.hidden}` | [A hidden link](URL){:.hidden} |
{:.headerless}

---

## Predefined Colors

|-----------------------------------------|---------------------------------------|
| `<span>Blue text</span>{:.blue}`        | <span>Blue text</span>{:.blue}        |
| `<span>Orange text</span>{:.orange}`    | <span>Orange text</span>{:.orange}    |
| `<span>Green text</span>{:.green}`      | <span>Green text</span>{:.green}      |
| `<span>Red text</span>{:.red}`          | <span>Red text</span>{:.red}          |
| `<span>Purple text</span>{:.purple}`    | <span>Purple text</span>{:.purple}    |
| `<span>Blue text</span>{:.hl-blue}`     | <span>Blue text</span>{:.hl-blue}     |
| `<span>Orange text</span>{:.hl-orange}` | <span>Orange text</span>{:.hl-orange} |
| `<span>Green text</span>{:.hl-green}`   | <span>Green text</span>{:.hl-green}   |
| `<span>Red text</span>{:.hl-red}`       | <span>Red text</span>{:.hl-red}       |
| `<span>Purple text</span>{:.hl-purple}` | <span>Purple text</span>{:.hl-purple} |
{:.headerless}

---

## Fonts

| Input                                             | Output                                          |
| ------------------------------------------------- | ----------------------------------------------- |
| `<span>This is a small font.</span>{:.small}`     | <span>This is a small font.</span>{:.small}     |
| `<span>This is a smaller font.</span>{:.smaller}` | <span>This is a smaller font.</span>{:.smaller} |
| `<span>This is a larger font.</span>{:.larger}`   | <span>This is a larger font.</span>{:.larger}   |
| `<span>These are weak texts.</span>{:.weak}`      | <span>These are weak texts.</span>{:.weak}      |
| `<span>These are details.</span>{:.detail}`       | <span>These are details.</span>{:.detail}       |
{:.headerless}

To apply a class selector like "`{:.small}`" to the whole paragraph, place it at the end of a paragraph, after a new line. For example,

```markdown
This is a small font.
{:.small}
```

---

## Centering Texts

- **Example input**:

  ```markdown
  Some centered texts
  {:.center}
  ```

  **Example output**:

  Some centered texts
  {:.center}

---

## Colored Block Quotes

You may apply a predefined color `{:.blue}`, `{:.orange}`, `{:.green}`, `{:.red}`, `{:.purple}` to a block quote. For example,

```markdown
> This is a red block quote.
{:.red}
```

will give:

> This is a red block quote.
{:.red}

To make it more visually prominent, you may add `{:.hl-blue}`, `{:.hl-orange}`, `{:.hl-green}`, `{:.hl-red}`, `{:.hl-purple}` to the class selector. For example,

```markdown
> This is a blue block quote.
{:.blue.hl-blue}
```

will give:

> This is a blue block quote.
{:.blue.hl-blue}

---

## Audio & Video Players

### Audio player

- **Format**: {% raw %}`{% include audio.html filename="FILENAME.EXT" %}`{% endraw %}\\
  **Example input**: {% raw %}`{% include audio.html filename="hw1/example_audio.mp3" %}`{% endraw %}\\
  **Example output**:

  {% include audio.html filename="hw1/example_audio.mp3" %}

### Video player

- **Format**: {% raw %}`{% include video.html filename="FILENAME.EXT" style="CSS_STYLE" %}`{% endraw %}\\
  **Example input**: {% raw %}`{% include video.html filename="hw1/example_video.mp4" style="max-width: 300px;" %}`{% endraw %}\\
  **Example output**:

  {% include video.html filename="hw1/example_video.mp4" style="max-width: 300px;" %}

### YouTube video player

- **Format**: {% raw %}`{% include youtube.html id="YOUTUBE_ID" t="START_TIME" %}`{% endraw %}\\
  **Example input**: {% raw %}`{% include youtube.html id="WJ1aIXL7F18" %}`{% endraw %}\\
  **Example output**:

  {% include youtube.html id="WJ1aIXL7F18" %}

---

## Math Support

- **Format**: `$FORMULA$`\\
  **Example input**: `Euler's equation: $e^{i x} = \cos(x) + i \sin(x)$`\\
  **Example output**: Euler's equation: $e^{i x} = \cos(x) + i \sin(x)$
- **Format**: `$$FORMULA$$`\\
  **Example input**: `$$P(A \mid B) = \frac{P(B \mid A) \cdot P(A)}{P(B)}$$`\\
  **Example output**:

  $$P(A \mid B) = \frac{P(B \mid A) \cdot P(A)}{P(B)}$$

---

## Icon Links

|------------------------------------------------------------------------|-------------------------------------------------|
| {% raw %}`{% include link.html link="#" %}`{% endraw %}                | {% include link.html link="#" %}                |
| {% raw %}`{% include link.html link="#" icon="file" %}`{% endraw %}    | {% include link.html link="#" icon="file" %}    |
| {% raw %}`{% include link.html link="#" icon="book" %}`{% endraw %}    | {% include link.html link="#" icon="book" %}    |
| {% raw %}`{% include link.html link="#" icon="folder" %}`{% endraw %}  | {% include link.html link="#" icon="folder" %}  |
| {% raw %}`{% include link.html link="#" icon="audio" %}`{% endraw %}   | {% include link.html link="#" icon="audio" %}   |
| {% raw %}`{% include link.html link="#" icon="video" %}`{% endraw %}   | {% include link.html link="#" icon="video" %}   |
| {% raw %}`{% include link.html link="#" icon="youtube" %}`{% endraw %} | {% include link.html link="#" icon="youtube" %} |
| {% raw %}`{% include link.html link="#" icon="code" %}`{% endraw %}    | {% include link.html link="#" icon="code" %}    |
| {% raw %}`{% include link.html link="#" icon="github" %}`{% endraw %}  | {% include link.html link="#" icon="github" %}  |
{:.headerless}

|----------------------------------------------------------------------------------------|-----------------------------------------------------------------|
| {% raw %}`{% include link.html link="#" text="link" %}`{% endraw %}                    | {% include link.html link="#" text="link" %}                    |
| {% raw %}`{% include link.html link="#" icon="file" text="slides" %}`{% endraw %}      | {% include link.html link="#" icon="file" text="slides" %}      |
| {% raw %}`{% include link.html link="#" icon="book" text="reading" %}`{% endraw %}     | {% include link.html link="#" icon="book" text="reading" %}     |
| {% raw %}`{% include link.html link="#" icon="folder" text="materials" %}`{% endraw %} | {% include link.html link="#" icon="folder" text="materials" %} |
| {% raw %}`{% include link.html link="#" icon="audio" text="audio" %}`{% endraw %}      | {% include link.html link="#" icon="audio" text="audio" %}      |
| {% raw %}`{% include link.html link="#" icon="video" text="video" %}`{% endraw %}      | {% include link.html link="#" icon="video" text="video" %}      |
| {% raw %}`{% include link.html link="#" icon="youtube" text="video" %}`{% endraw %}    | {% include link.html link="#" icon="youtube" text="video" %}    |
| {% raw %}`{% include link.html link="#" icon="code" text="code" %}`{% endraw %}        | {% include link.html link="#" icon="code" text="code" %}        |
| {% raw %}`{% include link.html link="#" icon="github" text="code" %}`{% endraw %}      | {% include link.html link="#" icon="github" text="code" %}      |
{:.headerless}

---

## Adjusting Element Widths

> The default image width is 600px.

- **Format**: `![Alt text](FILENAME.EXT){:style="CSS_STYLE"}`\\
  **Example input**: `![Winnie the Pooh and Christopher Robin](hw1/example_image.jpg){:style="max-width: 300px;"}`\\
  **Example output**:

  ![Winnie the Pooh and Christopher Robin](hw1/example_image.jpg){:style="max-width: 300px;"}

---

## Image Captions

> The `.caption` and `.caption-above` classes mainly make the captions center aligned and adjust the margins.

- **Example input**:

  ```markdown
  ![Winnie the Pooh and Christopher Robin](hw1/example_image.jpg)

  Winnie the Pooh and Christopher Robin
  {:.caption}
  ```

  **Example output**:

  ![Winnie the Pooh and Christopher Robin](hw1/example_image.jpg)

  Winnie the Pooh and Christopher Robin
  {:.caption}

- **Example input**:

  ```markdown
  Winnie the Pooh and Christopher Robin
  {:.caption-above}

  ![Winnie the Pooh and Christopher Robin](hw1/example_image.jpg)
  ```

  **Example output**:

  Winnie the Pooh and Christopher Robin
  {:.caption-above}

  ![Winnie the Pooh and Christopher Robin](hw1/example_image.jpg)

---

## Table Formatting

### Horizontally scrollable tables (most notable on smaller screens)

- **Example input**:

  ```markdown
  <div class="table-wrapper" markdown=1>

  | A                                                                                                                             | B                                                                                                           | C                                                                                                      | D                                                                                                              |
  | ----------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------- |
  | Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod   tempor incididunt ut labore et dolore magna aliqua. | Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. | Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. | Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum. |

  </div>
  ```

  **Example output**:

  <div class="table-wrapper" markdown=1>

  | A                                                                                                                             | B                                                                                                           | C                                                                                                      | D                                                                                                              |
  | ----------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------- |
  | Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod   tempor incididunt ut labore et dolore magna aliqua. | Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. | Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. | Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum. |

  </div>

### Tables without headers

- **Example input**:

  ```markdown
  |         |                 |
  | ------- | --------------- |
  | A table | without headers |
  | A table | without headers |
  {:.headerless}
  ```

  Example output:

  |         |                 |
  | ------- | --------------- |
  | A table | without headers |
  | A table | without headers |
  {:.headerless}

### Tables without borders

- **Example input**:

  ```markdown
  | A       | B               |
  | ------- | --------------- |
  | A table | without borders |
  | A table | without borders |
  | A table | without borders |
  {:.borderless}
  ```

  **Example output**:

  | A       | B               |
  | ------- | --------------- |
  | A table | without borders |
  | A table | without borders |
  | A table | without borders |
  {:.borderless}
