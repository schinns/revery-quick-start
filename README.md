[![Build Status](https://bryphe.visualstudio.com/revery-quick-start/_apis/build/status/build)](https://bryphe.visualstudio.com/revery-quick-start/_build/latest?definitionId=4)

# revery-quick-start

---

__Clone and run for a quick way to see Revery in action.__

This is a minimal Revery application to get you started.

The most important file here is:
- `app.re` - This is the core application code, responsible for __creating a window__ and __rendering__.

A Revery application also needs these files:
- `package.json` - [esy configuration]() - lists the OCaml/Reason dependencies.
- `dune` / `dune-project` - build configuration files used by [Dune](https://dune.readthedocs.io/en/latest/).
- `.opam` - metadata used by the build system.

### Prerequisites

- Install [Git](https://git-scm.com/)
- Install [Esy](https://esy.sh/)

### Build

- `esy install`
- `esy build`

The binary will be in the `_build/install/default/bin` - you can run it like:

- `_build/install/default/bin/App`

or with esy:

- `esy run`

```
# Clone the repository
git clone https://github.com/bryphe/revery-quick-start
# Go into the repository
cd revery-quick-start
# Install dependencies
esy install
# Build dependencies
esy build
# Run the app
esy run
```

> __NOTE:__ The first build will take a while - building the OCaml compiler and dependencies takes time! Subsequent builds, though, should be very fast.

### Resources

- Check out the [official reason docs](https://reasonml.github.io/docs/en/what-and-why) to learn more about reason
- Visit the Reason [discord channel](https://discordapp.com/invite/reasonml) and say hi!

### Next steps

Here's a few challenges to see if you've got the basics:

- Change the text from 'Hello World' to something more interesting!
- Add an Image component (Hint - you'll need to add the resource to the `dune` file, too)
- Respond to user input
- Create a frameless window

### License

[MIT License](LICENSE)
