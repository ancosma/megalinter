<!-- markdownlint-disable MD033 MD041 -->
<!-- @generated by .automation/build.py, please do not update manually -->

<div align="center">
  <a href="https://github.com/secretlint/secretlint#readme" target="blank" title="Visit linter Web Site">
    <img src="https://github.com/secretlint/secretlint/raw/master/docs/assets/SecretLintLP.png" alt="secretlint" height="150px" class="megalinter-banner">
  </a>
</div>

## secretlint documentation

- Version in Mega-Linter: **3.3.0**
- Visit [Official Web Site](https://github.com/secretlint/secretlint#readme){target=_blank}
- See [How to configure secretlint rules](https://github.com/secretlint/secretlint#configuration){target=_blank}
  - If custom `.secretlintrc.json` config file is not found, [.secretlintrc.json](https://github.com/nvuillam/mega-linter/tree/master/TEMPLATES/.secretlintrc.json){target=_blank} will be used
- See [Index of problems detected by secretlint](https://github.com/secretlint/secretlint#rule-packages){target=_blank}

[![secretlint - GitHub](https://gh-card.dev/repos/secretlint/secretlint.svg?fullname=)](https://github.com/secretlint/secretlint){target=_blank}

## Configuration in Mega-Linter

- Enable secretlint by adding `CREDENTIALS_SECRETLINT` in [ENABLE_LINTERS variable](https://nvuillam.github.io/mega-linter/configuration/#activation-and-deactivation)
- Disable secretlint by adding `CREDENTIALS_SECRETLINT` in [DISABLE_LINTERS variable](https://nvuillam.github.io/mega-linter/configuration/#activation-and-deactivation)

| Variable                                           | Description                                                                                                                                                                                  | Default value                                    |
|----------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------|
| CREDENTIALS_SECRETLINT_ARGUMENTS                   | User custom arguments to add in linter CLI call<br/>Ex: `-s --foo "bar"`                                                                                                                     |                                                  |
| CREDENTIALS_SECRETLINT_FILE_EXTENSIONS             | Allowed file extensions. `"*"` matches any extension, `""` matches empty extension. Empty list excludes all files<br/>Ex: `[".py", ""]`                                                      | Exclude every file                               |
| CREDENTIALS_SECRETLINT_FILE_NAMES_REGEX            | File name regex filters. Regular expression list for filtering files by their base names using regex full match. Empty list includes all files<br/>Ex: `["Dockerfile(-.+)?", "Jenkinsfile"]` | Include every file                               |
| CREDENTIALS_SECRETLINT_PRE_COMMANDS                | List of bash commands to run before the linter                                                                                                                                               | None                                             |
| CREDENTIALS_SECRETLINT_POST_COMMANDS               | List of bash commands to run after the linter                                                                                                                                                | None                                             |
| CREDENTIALS_SECRETLINT_CONFIG_FILE                 | secretlint configuration file name</br>Use `LINTER_DEFAULT` to let the linter find it                                                                                                        | `.secretlintrc.json`                             |
| CREDENTIALS_SECRETLINT_RULES_PATH                  | Path where to find linter configuration file                                                                                                                                                 | Workspace folder, then Mega-Linter default rules |
| CREDENTIALS_SECRETLINT_DISABLE_ERRORS              | Run linter but consider errors as warnings                                                                                                                                                   | `false`                                          |
| CREDENTIALS_SECRETLINT_DISABLE_ERRORS_IF_LESS_THAN | Maximum number of errors allowed                                                                                                                                                             | `0`                                              |

## Mega-Linter Flavours

This linter is available in the following flavours

|                                                                         <!-- -->                                                                          | Flavor                                                                         | Description                                           | Embedded linters |                                                                                                                                                                                               Info |
|:---------------------------------------------------------------------------------------------------------------------------------------------------------:|:-------------------------------------------------------------------------------|:------------------------------------------------------|:----------------:|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
| <img src="https://github.com/nvuillam/mega-linter/raw/master/docs/assets/images/mega-linter-square.png" alt="" height="32px" class="megalinter-icon"></a> | [all](https://nvuillam.github.io/mega-linter/supported-linters/)               | Default Mega-Linter Flavor                            |        93        |                             ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/nvuillam/mega-linter/v4) ![Docker Pulls](https://img.shields.io/docker/pulls/nvuillam/mega-linter) |
|        <img src="https://github.com/nvuillam/mega-linter/raw/master/docs/assets/icons/dart.ico" alt="" height="32px" class="megalinter-icon"></a>         | [dart](https://nvuillam.github.io/mega-linter/flavors/dart/)                   | Optimized for DART based projects                     |        40        |                   ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/nvuillam/mega-linter-dart/v4) ![Docker Pulls](https://img.shields.io/docker/pulls/nvuillam/mega-linter-dart) |
|    <img src="https://github.com/nvuillam/mega-linter/raw/master/docs/assets/icons/documentation.ico" alt="" height="32px" class="megalinter-icon"></a>    | [documentation](https://nvuillam.github.io/mega-linter/flavors/documentation/) | Mega-Linter for documentation projects                |        39        | ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/nvuillam/mega-linter-documentation/v4) ![Docker Pulls](https://img.shields.io/docker/pulls/nvuillam/mega-linter-documentation) |
|       <img src="https://github.com/nvuillam/mega-linter/raw/master/docs/assets/icons/dotnet.ico" alt="" height="32px" class="megalinter-icon"></a>        | [dotnet](https://nvuillam.github.io/mega-linter/flavors/dotnet/)               | Optimized for C, C++, C# or VB based projects         |        46        |               ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/nvuillam/mega-linter-dotnet/v4) ![Docker Pulls](https://img.shields.io/docker/pulls/nvuillam/mega-linter-dotnet) |
|         <img src="https://github.com/nvuillam/mega-linter/raw/master/docs/assets/icons/go.ico" alt="" height="32px" class="megalinter-icon"></a>          | [go](https://nvuillam.github.io/mega-linter/flavors/go/)                       | Optimized for GO based projects                       |        41        |                       ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/nvuillam/mega-linter-go/v4) ![Docker Pulls](https://img.shields.io/docker/pulls/nvuillam/mega-linter-go) |
|        <img src="https://github.com/nvuillam/mega-linter/raw/master/docs/assets/icons/java.ico" alt="" height="32px" class="megalinter-icon"></a>         | [java](https://nvuillam.github.io/mega-linter/flavors/java/)                   | Optimized for JAVA based projects                     |        41        |                   ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/nvuillam/mega-linter-java/v4) ![Docker Pulls](https://img.shields.io/docker/pulls/nvuillam/mega-linter-java) |
|     <img src="https://github.com/nvuillam/mega-linter/raw/master/docs/assets/icons/javascript.ico" alt="" height="32px" class="megalinter-icon"></a>      | [javascript](https://nvuillam.github.io/mega-linter/flavors/javascript/)       | Optimized for JAVASCRIPT or TYPESCRIPT based projects |        48        |       ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/nvuillam/mega-linter-javascript/v4) ![Docker Pulls](https://img.shields.io/docker/pulls/nvuillam/mega-linter-javascript) |
|         <img src="https://github.com/nvuillam/mega-linter/raw/master/docs/assets/icons/php.ico" alt="" height="32px" class="megalinter-icon"></a>         | [php](https://nvuillam.github.io/mega-linter/flavors/php/)                     | Optimized for PHP based projects                      |        43        |                     ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/nvuillam/mega-linter-php/v4) ![Docker Pulls](https://img.shields.io/docker/pulls/nvuillam/mega-linter-php) |
|       <img src="https://github.com/nvuillam/mega-linter/raw/master/docs/assets/icons/python.ico" alt="" height="32px" class="megalinter-icon"></a>        | [python](https://nvuillam.github.io/mega-linter/flavors/python/)               | Optimized for PYTHON based projects                   |        48        |               ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/nvuillam/mega-linter-python/v4) ![Docker Pulls](https://img.shields.io/docker/pulls/nvuillam/mega-linter-python) |
|        <img src="https://github.com/nvuillam/mega-linter/raw/master/docs/assets/icons/ruby.ico" alt="" height="32px" class="megalinter-icon"></a>         | [ruby](https://nvuillam.github.io/mega-linter/flavors/ruby/)                   | Optimized for RUBY based projects                     |        40        |                   ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/nvuillam/mega-linter-ruby/v4) ![Docker Pulls](https://img.shields.io/docker/pulls/nvuillam/mega-linter-ruby) |
|        <img src="https://github.com/nvuillam/mega-linter/raw/master/docs/assets/icons/rust.ico" alt="" height="32px" class="megalinter-icon"></a>         | [rust](https://nvuillam.github.io/mega-linter/flavors/rust/)                   | Optimized for RUST based projects                     |        40        |                   ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/nvuillam/mega-linter-rust/v4) ![Docker Pulls](https://img.shields.io/docker/pulls/nvuillam/mega-linter-rust) |
|     <img src="https://github.com/nvuillam/mega-linter/raw/master/docs/assets/icons/salesforce.ico" alt="" height="32px" class="megalinter-icon"></a>      | [salesforce](https://nvuillam.github.io/mega-linter/flavors/salesforce/)       | Optimized for Salesforce based projects               |        42        |       ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/nvuillam/mega-linter-salesforce/v4) ![Docker Pulls](https://img.shields.io/docker/pulls/nvuillam/mega-linter-salesforce) |
|        <img src="https://github.com/nvuillam/mega-linter/raw/master/docs/assets/icons/scala.ico" alt="" height="32px" class="megalinter-icon"></a>        | [scala](https://nvuillam.github.io/mega-linter/flavors/scala/)                 | Optimized for SCALA based projects                    |        40        |                 ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/nvuillam/mega-linter-scala/v4) ![Docker Pulls](https://img.shields.io/docker/pulls/nvuillam/mega-linter-scala) |
|        <img src="https://github.com/nvuillam/mega-linter/raw/master/docs/assets/icons/swift.ico" alt="" height="32px" class="megalinter-icon"></a>        | [swift](https://nvuillam.github.io/mega-linter/flavors/swift/)                 | Optimized for SWIFT based projects                    |        40        |                 ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/nvuillam/mega-linter-swift/v4) ![Docker Pulls](https://img.shields.io/docker/pulls/nvuillam/mega-linter-swift) |
|      <img src="https://github.com/nvuillam/mega-linter/raw/master/docs/assets/icons/terraform.ico" alt="" height="32px" class="megalinter-icon"></a>      | [terraform](https://nvuillam.github.io/mega-linter/flavors/terraform/)         | Optimized for TERRAFORM based projects                |        44        |         ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/nvuillam/mega-linter-terraform/v4) ![Docker Pulls](https://img.shields.io/docker/pulls/nvuillam/mega-linter-terraform) |

## Behind the scenes

### How are identified applicable files

- If this linter is active, all files will always be linted

<!-- markdownlint-disable -->
<!-- /* cSpell:disable */ -->
### How the linting is performed

secretlint is called once on the whole project directory

- filtering can not be done using Mega-Linter configuration variables,it must be done using secretlint configuration or ignore file (if existing)
- `VALIDATE_ALL_CODEBASE: false` does not make secretlint analyze only updated files

### Example calls

```shell
secretlint "*/**"
```

```shell
secretlint --secretlintrc .secretlintrc.json "**/*"
```


### Help content

```shell

  Secretlint CLI that scan secret/credential data.

  Usage
    $ secretlint [file|glob*]

  Note
    supported glob syntax is based on microglob
    https://github.com/micromatch/micromatch#matching-features

  Options
    --init             setup config file. Create .secretlintrc.json file from your package.json
    --format           [String] formatter name. Default: "stylish". Available Formatter: checkstyle, compact, jslint-xml, json, junit, pretty-error, stylish, tap, unix, table.d, table
    --output           [path:String] output file path that is written of reported result.
    --no-color         disable ANSI-color of output.
    --no-terminalLink  disable terminalLink of output.
    --maskSecrets      enable masking of secret values. replace actual secrets with "***".
    --secretlintrc     [path:String] path to .secretlintrc config file. Default: .secretlintrc.*
    --secretlintignore [path:String] path to .secretlintignore file. Default: .secretlintignore

  Options for Developer
    --profile          Enable performance profile.
    --secretlintrcJSON [String] a JSON string of .secretlintrc. use JSON string instead of rc file.

  Experimental Options
    --locale            [String] locale tag for translating message. Default: en

  Examples
    $ secretlint ./README.md
    # glob pattern should be wrapped with double quote
    $ secretlint "**/*"
    $ secretlint "source/**/*.ini"

```

### Installation on mega-linter Docker image

- NPM packages (node.js):
  - [secretlint](https://www.npmjs.com/package/secretlint)
  - [@secretlint/secretlint-rule-preset-recommend](https://www.npmjs.com/package/@secretlint/secretlint-rule-preset-recommend)