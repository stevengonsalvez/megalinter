<!-- markdownlint-disable MD033 MD041 -->
<!-- @generated by .automation/build.py, please do not update manually -->

<div align="center">
  <a href="https://github.com/yannickcr/eslint-plugin-react#readme" target="blank" title="Visit linter Web Site">
    <img src="https://d33wubrfki0l68.cloudfront.net/3b5ac7586466159bb6f237b633bfc4f5a8d5acf8/ee0a1/assets/img/posts/eslint-collective.png" alt="eslint" height="150px" class="megalinter-banner">
  </a>
</div>

eslint requires a custom configuration file applicable to your project.
You can create it by typing `npx eslint --init` in the root of your repository

## eslint documentation

- Version in MegaLinter: **8.9.0**
- Visit [Official Web Site](https://github.com/yannickcr/eslint-plugin-react#readme){target=_blank}
- See [How to configure eslint rules](https://github.com/yannickcr/eslint-plugin-react#configuration){target=_blank}
- See [How to disable eslint rules in files](https://eslint.org/docs/user-guide/configuring#disabling-rules-with-inline-comments){target=_blank}
- See [Index of problems detected by eslint](https://github.com/yannickcr/eslint-plugin-react#list-of-supported-rules){target=_blank}

[![eslint-plugin-react - GitHub](https://gh-card.dev/repos/yannickcr/eslint-plugin-react.svg?fullname=)](https://github.com/yannickcr/eslint-plugin-react){target=_blank}

## Configuration in MegaLinter

- Enable eslint by adding `JSX_ESLINT` in [ENABLE_LINTERS variable](https://megalinter.github.io/configuration/#activation-and-deactivation)
- Disable eslint by adding `JSX_ESLINT` in [DISABLE_LINTERS variable](https://megalinter.github.io/configuration/#activation-and-deactivation)

- Enable **auto-fixes** by adding `JSX_ESLINT` in [APPLY_FIXES variable](https://megalinter.github.io/configuration/#apply-fixes)

| Variable                               | Description                                                                                                                                                                                                         | Default value                                   |
|----------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------|
| JSX_ESLINT_ARGUMENTS                   | User custom arguments to add in linter CLI call<br/>Ex: `-s --foo "bar"`                                                                                                                                            |                                                 |
| JSX_ESLINT_FILTER_REGEX_INCLUDE        | Custom regex including filter<br/>Ex: `(src\|lib)`                                                                                                                                                                  | Include every file                              |
| JSX_ESLINT_FILTER_REGEX_EXCLUDE        | Custom regex excluding filter<br/>Ex: `(test\|examples)`                                                                                                                                                            | Exclude no file                                 |
| JSX_ESLINT_CLI_LINT_MODE               | Override default CLI lint mode<br/>- `file`: Calls the linter for each file<br/>- `list_of_files`: Call the linter with the list of files as argument<br/>- `project`: Call the linter from the root of the project | `list_of_files`                                 |
| JSX_ESLINT_FILE_EXTENSIONS             | Allowed file extensions. `"*"` matches any extension, `""` matches empty extension. Empty list excludes all files<br/>Ex: `[".py", ""]`                                                                             | `[".jsx"]`                                      |
| JSX_ESLINT_FILE_NAMES_REGEX            | File name regex filters. Regular expression list for filtering files by their base names using regex full match. Empty list includes all files<br/>Ex: `["Dockerfile(-.+)?", "Jenkinsfile"]`                        | Include every file                              |
| JSX_ESLINT_PRE_COMMANDS                | List of bash commands to run before the linter                                                                                                                                                                      | None                                            |
| JSX_ESLINT_POST_COMMANDS               | List of bash commands to run after the linter                                                                                                                                                                       | None                                            |
| JSX_ESLINT_CONFIG_FILE                 | eslint configuration file name</br>Use `LINTER_DEFAULT` to let the linter find it                                                                                                                                   | `.eslintrc.json`                                |
| JSX_ESLINT_RULES_PATH                  | Path where to find linter configuration file                                                                                                                                                                        | Workspace folder, then MegaLinter default rules |
| JSX_ESLINT_DISABLE_ERRORS              | Run linter but consider errors as warnings                                                                                                                                                                          | `false`                                         |
| JSX_ESLINT_DISABLE_ERRORS_IF_LESS_THAN | Maximum number of errors allowed                                                                                                                                                                                    | `0`                                             |

## IDE Integration

Use eslint in your favorite IDE to catch errors before MegaLinter !

|                                                                   <!-- -->                                                                    | IDE                                                      | Extension Name                                                                                 |                                                                                   Install                                                                                   |
|:---------------------------------------------------------------------------------------------------------------------------------------------:|----------------------------------------------------------|------------------------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
|   <img src="https://github.com/megalinter/megalinter/raw/main/docs/assets/icons/atom.ico" alt="" height="32px" class="megalinter-icon"></a>   | [Atom](https://atom.io/)                                 | [linter-eslint](https://atom.io/packages/linter-eslint)                                        |                                                   [Visit Web Site](https://atom.io/packages/linter-eslint){target=_blank}                                                   |
| <img src="https://github.com/megalinter/megalinter/raw/main/docs/assets/icons/brackets.ico" alt="" height="32px" class="megalinter-icon"></a> | [Brackets](http://brackets.io/)                          | [brackets-eslint](https://github.com/brackets-userland/brackets-eslint)                        |                                            [Visit Web Site](https://github.com/brackets-userland/brackets-eslint){target=_blank}                                            |
| <img src="https://github.com/megalinter/megalinter/raw/main/docs/assets/icons/eclipse.ico" alt="" height="32px" class="megalinter-icon"></a>  | [Eclipse](https://www.eclipse.org/)                      | [Tern-Linter-ESLint](https://github.com/angelozerr/tern.java/wiki/Tern-Linter-ESLint)          |                                      [Visit Web Site](https://github.com/angelozerr/tern.java/wiki/Tern-Linter-ESLint){target=_blank}                                       |
|  <img src="https://github.com/megalinter/megalinter/raw/main/docs/assets/icons/emacs.ico" alt="" height="32px" class="megalinter-icon"></a>   | [Emacs](https://www.gnu.org/software/emacs/)             | [flycheck](http://www.flycheck.org/en/latest/languages.html#javascript)                        |                                        [Visit Web Site](http://www.flycheck.org/en/latest/languages.html#javascript){target=_blank}                                         |
|   <img src="https://github.com/megalinter/megalinter/raw/main/docs/assets/icons/idea.ico" alt="" height="32px" class="megalinter-icon"></a>   | [IDEA](https://www.jetbrains.com/products.html#type=ide) | [ESLint Plugin](https://plugins.jetbrains.com/plugin/7494-eslint)                              |                        <iframe frameborder="none" width="245px" height="48px" src="https://plugins.jetbrains.com/embeddable/install/7494"></iframe>                         |
| <img src="https://github.com/megalinter/megalinter/raw/main/docs/assets/icons/sublime.ico" alt="" height="32px" class="megalinter-icon"></a>  | [Sublime Text](https://www.sublimetext.com/)             | [SublimeLinter-eslint](https://github.com/roadhump/SublimeLinter-eslint)                       |                                              [Visit Web Site](https://github.com/roadhump/SublimeLinter-eslint){target=_blank}                                              |
|   <img src="https://github.com/megalinter/megalinter/raw/main/docs/assets/icons/vim.ico" alt="" height="32px" class="megalinter-icon"></a>    | [vim](https://www.vim.org/)                              | [ale](https://github.com/w0rp/ale)                                                             |                                                        [Visit Web Site](https://github.com/w0rp/ale){target=_blank}                                                         |
|   <img src="https://github.com/megalinter/megalinter/raw/main/docs/assets/icons/vim.ico" alt="" height="32px" class="megalinter-icon"></a>    | [vim](https://www.vim.org/)                              | [Syntastic](https://github.com/vim-syntastic/syntastic/tree/master/syntax_checkers/javascript) |                             [Visit Web Site](https://github.com/vim-syntastic/syntastic/tree/master/syntax_checkers/javascript){target=_blank}                              |
|  <img src="https://github.com/megalinter/megalinter/raw/main/docs/assets/icons/vscode.ico" alt="" height="32px" class="megalinter-icon"></a>  | [Visual Studio Code](https://code.visualstudio.com/)     | [vscode-eslint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)    | [![Install in VsCode](https://github.com/megalinter/megalinter/raw/main/docs/assets/images/btn_install_vscode.png)](vscode:extension/dbaeumer.vscode-eslint){target=_blank} |

## MegaLinter Flavours

This linter is available in the following flavours

|                                                                         <!-- -->                                                                         | Flavor                                                         | Description                                           | Embedded linters |                                                                                                                                                                                           Info |
|:--------------------------------------------------------------------------------------------------------------------------------------------------------:|:---------------------------------------------------------------|:------------------------------------------------------|:----------------:|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
| <img src="https://github.com/megalinter/megalinter/raw/main/docs/assets/images/mega-linter-square.png" alt="" height="32px" class="megalinter-icon"></a> | [all](https://megalinter.github.io/supported-linters/)         | Default MegaLinter Flavor                             |        96        |                       ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/megalinter/megalinter/v5) ![Docker Pulls](https://img.shields.io/docker/pulls/megalinter/megalinter) |
|     <img src="https://github.com/megalinter/megalinter/raw/main/docs/assets/icons/javascript.ico" alt="" height="32px" class="megalinter-icon"></a>      | [javascript](https://megalinter.github.io/flavors/javascript/) | Optimized for JAVASCRIPT or TYPESCRIPT based projects |        48        | ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/megalinter/megalinter-javascript/v5) ![Docker Pulls](https://img.shields.io/docker/pulls/megalinter/megalinter-javascript) |

## Behind the scenes

### How are identified applicable files

- Activated only if one of these files is found: `.eslintrc.json, .eslintrc.yml, .eslintrc.yaml, .eslintrc.js, .eslintrc.cjs, package.json:eslintConfig`
- File extensions: `.jsx`

<!-- markdownlint-disable -->
<!-- /* cSpell:disable */ -->
### How the linting is performed

- eslint is called once with the list of files as arguments

### Example calls

```shell
eslint myfile.jsx
```

```shell
eslint -c .eslintrc.json --no-eslintrc --no-ignore myfile.jsx
```

```shell
eslint --fix -c .eslintrc.json --no-eslintrc --no-ignore myfile.jsx
```


### Help content

```shell
eslint [options] file.js [file.js] [dir]

Basic configuration:
  --no-eslintrc                   Disable use of configuration from .eslintrc.*
  -c, --config path::String       Use this configuration, overriding .eslintrc.* config options if present
  --env [String]                  Specify environments
  --ext [String]                  Specify JavaScript file extensions
  --global [String]               Define global variables
  --parser String                 Specify the parser to be used
  --parser-options Object         Specify parser options
  --resolve-plugins-relative-to path::String  A folder where plugins should be resolved from, CWD by default

Specifying rules and plugins:
  --plugin [String]               Specify plugins
  --rule Object                   Specify rules
  --rulesdir [path::String]       Load additional rules from this directory. Deprecated: Use rules from plugins

Fixing problems:
  --fix                           Automatically fix problems
  --fix-dry-run                   Automatically fix problems without saving the changes to the file system
  --fix-type Array                Specify the types of fixes to apply (directive, problem, suggestion, layout)

Ignoring files:
  --ignore-path path::String      Specify path of ignore file
  --no-ignore                     Disable use of ignore files and patterns
  --ignore-pattern [String]       Pattern of files to ignore (in addition to those in .eslintignore)

Using stdin:
  --stdin                         Lint code provided on <STDIN> - default: false
  --stdin-filename String         Specify filename to process STDIN as

Handling warnings:
  --quiet                         Report errors only - default: false
  --max-warnings Int              Number of warnings to trigger nonzero exit code - default: -1

Output:
  -o, --output-file path::String  Specify file to write report to
  -f, --format String             Use a specific output format - default: stylish
  --color, --no-color             Force enabling/disabling of color

Inline configuration comments:
  --no-inline-config              Prevent comments from changing config or rules
  --report-unused-disable-directives  Adds reported errors for unused eslint-disable directives

Caching:
  --cache                         Only check changed files - default: false
  --cache-file path::String       Path to the cache file. Deprecated: use --cache-location - default: .eslintcache
  --cache-location path::String   Path to the cache file or directory
  --cache-strategy String         Strategy to use for detecting changed files in the cache - either: metadata or content - default: metadata

Miscellaneous:
  --init                          Run config initialization wizard - default: false
  --env-info                      Output execution environment information - default: false
  --no-error-on-unmatched-pattern  Prevent errors when pattern is unmatched
  --exit-on-fatal-error           Exit with exit code 2 in case of fatal error - default: false
  --debug                         Output debugging information
  -h, --help                      Show help
  -v, --version                   Output the version number
  --print-config path::String     Print the configuration for the given file
```

### Installation on mega-linter Docker image

- NPM packages (node.js):
  - [eslint](https://www.npmjs.com/package/eslint)
  - [eslint-plugin-react](https://www.npmjs.com/package/eslint-plugin-react)
  - [eslint-plugin-jsx-a11y](https://www.npmjs.com/package/eslint-plugin-jsx-a11y)

### Example success log

```shell
Results of eslint linter (version 7.15.0)
See documentation on https://megalinter.github.io/descriptors/jsx_eslint/
-----------------------------------------------

[SUCCESS] .automation/test/jsx/jsx_good_1.jsx
    Warning: React version not specified in eslint-plugin-react settings. See https://github.com/yannickcr/eslint-plugin-react#configuration .

```

### Example error log

```shell
Results of eslint linter (version 7.15.0)
See documentation on https://megalinter.github.io/descriptors/jsx_eslint/
-----------------------------------------------

[ERROR] .automation/test/jsx/jsx_bad_1.jsx
    
    .automation/test/jsx/jsx_bad_1.jsx
      8:1  error  Parsing error: Unexpected token const
    
    ✖ 1 problem (1 error, 0 warnings)

```
