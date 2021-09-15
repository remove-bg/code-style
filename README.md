# 🧑‍💻 kaleido.ai Code Style Guide

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
