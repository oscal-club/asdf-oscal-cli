# asdf-oscal-cli

[`oscal-cli`](https://github.com/usnistgov/oscal-cli.git)
plugin for the [asdf](https://github.com/asdf-vm/asdf) version manager.

## Install

After installing [asdf](https://github.com/asdf-vm/asdf),
you can add this plugin like this:

```bash
asdf plugin-add oscal-cli https://github.com/xee5ch/asdf-oscal-cli.git
```

and install new versions like this:

```bash
asdf install oscal-cli 0.2.0
```

and switch versions like this:

```bash
asdf global oscal-cli 0.1.0
```

## Configuration

### Configuring on macOS, maybe with a JRE installed from Homebrew, but it doesn't work?

Are you using `asdf` on macOS and having trouble with this plugin? If so, I will guess you are using Homebrew or another to tool to override the older, default installation of the Java Runtime Environment on your macOS. Is this the case for your workstation? 

If so, you need to explicitly override the path to the JRE or `oscal-cli` will look for the default one.

```
# This is the default for Homebrew, and may not be correct in all cases, so plan accordingly or ask for help.
# In your shell configuration file, be it ~/.bash_profile or ~/.zshrc:
export JAVA_HOME=/opt/homebrew/opt/openjdk
```

Thanks to the community member who pointed this out. See their report and explanation of this workaround in [xee5ch/asdf-oscal-cli#3](https://github.com/xee5ch/asdf-oscal-cli/issues/3) for more details.

## Reading

Read the [asdf readme](https://github.com/asdf-vm/asdf)
for instructions on how to install and manage versions of any language.

If you have trouble with any expected features,
have any feature requests or want to contribute,
please [do an issue](https://github.com/skotchpine/asdf-maven/issues).

## Development

- asdf's [creating-plugins.md](https://github.com/asdf-vm/asdf/blob/master/docs/creating-plugins.md)
- [Bash Hackers Wiki](http://wiki.bash-hackers.org/)
