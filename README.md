# Biome Plugin Maven

Provides number of handy functions to use in your plan

## Usage

```
pkg_build_deps+=(biome/bio-plugin-maven)

# Read version from pom.xml
pkg_version() {
  pkg_maven_version
}

do_setup_environment() {
  source "$(pkg_path_for biome/bio-plugin-maven)/lib/plugin.sh"

  # Set maven repository into studio cache
  do_maven_setup_cache
}
```

Consider source [bio-plugin-maven](habitat/lib/plugin.sh)
