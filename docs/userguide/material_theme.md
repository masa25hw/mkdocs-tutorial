# Material for MkDocs

## Configuration
This configuration enables abbreviations and allows to build a simple project-wide glossary, sourcing definitions from a central location. Add the following line to `mkdocs.yml`:

```
markdown_extensions:
  - abbr
  - pymdownx.snippets
```

`note`

!!! note
    note のサンプル表示

`abstract`, `summary`, `tldr`

!!! abstract
    abstract のサンプル表示

`info`, `todo`

!!! info
    info のサンプル表示

`tip`, `hint`, `important`

!!! tip
    tip のサンプル表示

`success`, `check`, `done`

!!! success
    success のサンプル表示

`question`, `help`, `faq`

!!! question
    question のサンプル表示


`warning`, `caution`, `attention`

!!! warning
    warning のサンプル表示

`failure`, `fail`, `missing`

!!! failure
    failure のサンプル表示

`danger`, `error`

!!! danger
    danger のサンプル表示

`bug`

!!! bug
    bug のサンプル表示
    hogehoge
    fugafuga

`example`

!!! example

    === "Unordered List"

        ``` markdown title="List, unordered"
        * Sed sagittis eleifend rutrum
        * Donec vitae suscipit est
        * Nulla tempor lobortis orci
        ```

    === "Ordered List"

        ``` markdown title="List, ordered"
        1. Sed sagittis eleifend rutrum
        2. Donec vitae suscipit est
        3. Nulla tempor lobortis orci
        ```


`quote`, `cite`

!!! quote
    quote のサンプル表示


++ctrl+alt+del++

## タブ
=== "Unordered list"

    * Sed sagittis eleifend rutrum
    * Donec vitae suscipit est
    * Nulla tempor lobortis orci

=== "Ordered list"

    1. Sed sagittis eleifend rutrum
    2. Donec vitae suscipit est
    3. Nulla tempor lobortis orci

他にも、

=== "C"
    C のサンプルコード
    ``` c
    #include <stdio.h>

    int main(void) {
      printf("Hello world!\n");
      return 0;
    }
    ```

=== "C++"
    C++ のサンプルコード

    ``` c++
    #include <iostream>

    int main(void) {
      std::cout << "Hello world!" << std::endl;
      return 0;
    }
    ```

インライン表示

=== "info inline end"
    ```
    !!! info inline end

        Lorem ipsum dolor sit amet, consectetur
        adipiscing elit. Nulla et euismod nulla.
        Curabitur feugiat, tortor non consequat
        finibus, justo purus auctor massa, nec
        semper lorem quam in massa.
    ```

    !!! info inline end

        Lorem ipsum dolor sit amet, consectetur
        adipiscing elit. Nulla et euismod nulla.
        Curabitur feugiat, tortor non consequat
        finibus, justo purus auctor massa, nec
        semper lorem quam in massa.

=== "info inline"
    ```
    !!! info inline

        Lorem ipsum dolor sit amet, consectetur
        adipiscing elit. Nulla et euismod nulla.
        Curabitur feugiat, tortor non consequat
        finibus, justo purus auctor massa, nec
        semper lorem quam in massa.
    ```

    !!! info inline

        Lorem ipsum dolor sit amet, consectetur
        adipiscing elit. Nulla et euismod nulla.
        Curabitur feugiat, tortor non consequat
        finibus, justo purus auctor massa, nec
        semper lorem quam in massa.


## Emoji

- [Material Design](https://materialdesignicons.com/)
- [FontAwesome](https://fontawesome.com/search?m=free)
    - [squidfunk/mkdocs-material](https://github.com/squidfunk/mkdocs-material/tree/master/material/.icons)
- [Octicons](https://primer.style/octicons)

:smile:

:fontawesome-regular-face-laugh-wink:

:fontawesome-regular-heart:

:fontawesome-brands-twitter:{ .twitter }

:octicons-heart-fill-24:{ .heart }