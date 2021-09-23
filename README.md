# 🧑‍💻 kaleido.ai Code Style Guide

## EditorConfig

We use [EditorConfig](https://editorconfig.org), which helps maintain consistent coding styles for multiple developers 
working on the same project across various editors and IDEs. The EditorConfig project consists of a file format for 
defining coding styles and a collection of text editor plugins that enable editors to read the file format and adhere 
to defined styles. EditorConfig files are easily readable and they work nicely with version control systems.

Our base [`.editorconfig`](.editorconfig) file can be copied to every repository.

## Ruby / Ruby on Rails

To use the Ruby/Rails code style with [Rubocop](https://github.com/rubocop/rubocop), create a `.rubocop.yml`
file in the root of your project and add the following:

```yaml
inherit_from: https://raw.githubusercontent.com/remove-bg/code-style/main/ruby/.rubocop-rails.yml

Bundler/OrderedGems:
  Enabled: yes

Rails/UnknownEnv:
  Environments:
    - production
    - staging
    - development
    - test
```

For pure Ruby code, create a `.rubocop.yml` file in the root of your project like this:

```yaml
inherit_from: https://raw.githubusercontent.com/remove-bg/code-style/main/ruby/.rubocop.yml

Metrics/BlockLength:
  Enabled: true
```
