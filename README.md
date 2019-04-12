# chromium_build

# command log
```bash
git clone https://chromium.googlesource.com/chromium/tools/depot_tools.git
export PATH="$PATH:$(pwd)/depot_tools"
git config --global core.precomposeUnicode true
mkdir chromium && cd chromium
fetch chromium
cd src
gn gen out/Default
brew install --HEAD ccache
autoninja -C out/Default chrome
```

# last log memo

```
Running hooks: 100% (74/74), done.
Running: git submodule foreach 'git config -f $toplevel/.git/config submodule.$name.ignore all'
Running: git config --add remote.origin.fetch '+refs/tags/*:refs/tags/*'
Running: git config diff.ignoreSubmodules all
```

# ref
https://chromium.googlesource.com/chromium/src.git/+/HEAD/docs/mac_build_instructions.md
