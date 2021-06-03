Note: We've forked this buildpack to help mitigate the risk of a
[supply chain attack](https://en.wikipedia.org/wiki/Supply_chain_attack)
where applications can become compromised via the compromised repo of a
third-party buildpack.

Big thanks to [Hirotaka Ikoma](https://github.com/hikoma) for making this
available to the Epihub, Inc. team.

---

# heroku-buildpack-cleanup

Remove files that are specified in a .slugcleanup file.

## Usage

    $ heroku buildpacks:add https://github.com/syginc/heroku-buildpack-cleanup.git

    $ cat .slugcleanup
    gradle*
    node_modules

## License

MIT
