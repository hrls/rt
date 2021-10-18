# rt
rust template

[![rust pipeline](https://github.com/hrls/rt/actions/workflows/rust.yml/badge.svg)](https://github.com/hrls/rt/actions/workflows/rust.yml)

```zsh
vared -p 'package name: ' -c package \
    && git clone -- git@github.com:hrls/rt.git ${package} \
    && cd ${package} \
    && cargo init --name $(basename $PWD) --bin -- $PWD \
    && cargo test \
    && cargo run
```
