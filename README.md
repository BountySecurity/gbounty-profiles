<h1 align="center">
  <br>
  <a href="https://gbounty.bountysecurity.ai/">
        <img src="static/gbounty-logo.png" width="800px" alt="GBounty">
  </a>
</h1>

<h4 align="center">Web vulnerability profiles.</h4>

<p align="center">
<a href="https://twitter.com/GBountySecurity"><img src="https://img.shields.io/twitter/follow/GBountySecurity.svg?logo=twitter"></a>
</p>

<p align="center">
  •
  <a href="#profiles">Profiles</a> •
</p>

---

Highly customizable website vulnerability profiles.

This repository houses various type of web vulnerability profiles contributed by security researchers and engineers.

> [!WARNING]  
> **This project is in active development.** 

## Profiles

### What is a profile?

A **profile** is a manifest file, in JSON format, with the `.bb2` extension, that contains all the information used
by [GBounty](https://github.com/BountySecurity/gbounty) to run web vulnerability scans.

### How can I use profiles?

By default, [GBounty](https://github.com/BountySecurity/gbounty) will download (clone) the latest release of this
repository, containing the most recent version of each profile, and store them in the `~/.gbounty/profiles` directory.

Later, whenever a new release is published, you can update them with: `gbounty --update-profiles`.

<br/>

Additionally, you can tell GBounty to use one (or more) specific profiles, with the `-p <path-to-profile>` flag.
For instance, in case you want to use just one profile: `gbounty -p ~/.gbounty/profiles/SQLi.bb2`. Or, in case
you want to manage your own set of profiles in another directory.

### How can I create new profiles?

To simplify the task of creating new profiles, and not having to write them manually in plain JSON, you can use
the [GBounty Profiles Designer](https://github.com/BountySecurity/GBountyProfilesDesigner/tree/master), which is
a small Java application with a user-friendly interface to create web vulnerability profiles.

Find [here](https://gbounty.bountysecurity.ai/gbounty-profiles-designer) the designer docs.
<br/>

And bear in mind, **contributions are welcome!**
<br/>
<br/>
<br/>

### License

GBounty Profiles are distributed under [MIT License](./LICENSE)
