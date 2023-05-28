# asdf-oscal-cli

[`oscal-cli`](https://github.com/usnistgov/oscal-cli.git)
plugin for the [asdf](https://github.com/asdf-vm/asdf) version manager.

## Install

After installing [asdf](https://github.com/asdf-vm/asdf),
you can add this plugin like this:

```bash
asdf plugin-add oscal-cli https://github.com/oscal-club/asdf-oscal-cli.git
```

and install new versions like this:

```bash
asdf install oscal-cli 0.3.3
```

and switch versions like this:

```bash
asdf global oscal-cli 0.3.2
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

Thanks to the community member who pointed this out. See their report and explanation of this workaround in [oscal-club/asdf-oscal-cli#3](https://github.com/xee5ch/asdf-oscal-cli/issues/3) for more details.

