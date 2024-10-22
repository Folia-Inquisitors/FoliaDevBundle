# FoliaDevBundle

A Maven Repository for supplying the Folia `dev-bundle`, mostly used for constructing Folia dependencies for some specialized plugins that rely on its internal APIs.

## Why?

Although PaperMC has a similar Maven repository exactly for this, they are slow on providing us with the necessary `dev-bundle` when a new MC version is released. After research on their publish workflow, we decided to make our own repository so that we can update our plugins faster for the new MC versions. Personally, this is for [MoreFoWorld](https://github.com/Folia-Inquisitors/MoreFoWorld), but this can also be useful for our future projects.

## Usage

```kts
repositories {
    maven {
        name = "folia-inquistors-repo"
        url = "https://folia-inquisitors.github.io/FoliaDevBundle/"
    }
    // Your other repositories
}
```
