### Prerequisites

You're going to need:

 - **Linux or OS X** -- Windows may work, but is unsupported.
 - **Ruby, version 2.2.5 or newer**
 - **Bundler** -- If Ruby is already installed, but the `bundle` command doesn't work, just run `gem install bundler` in a terminal.

### Getting Set Up

1. Fork this repository on Github.
2. Clone *your forked repository* (not our original one) to your hard drive with `git clone https://github.com/YOURUSERNAME/api-doc.git`
3. `cd api-doc`
4. Initialize and start API doc.

```shell
# either run this to run locally
bundle install
bundle exec middleman server
```

You can now see the docs at http://localhost:4567. Whoa! That was fast!