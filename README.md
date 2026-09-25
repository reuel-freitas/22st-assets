# 22st-assets

The demo photography, video and audio for the [21st.rails](https://github.com/reuel-freitas/22st)
component catalogue.

These files are the *defaults* the ported 21st.dev components render with. They live here rather
than in the code repository because Git keeps every version of every file forever: hundreds of
megabytes of binaries would make the code repository heavier with each category ported, and none
of it is code.

Paths mirror the logical asset path (`twentyfirst/demo/21st/<author>/<slug>/<file>`), which is also
what `Twentyfirst::DemoAssetHost` builds its fallback URLs from. `manifest.json` records which
`app/assets` directory each file belongs in.

Sync from the code repository:

    bin/sync-demo-assets              # fetch into app/assets
    bin/sync-demo-assets --publish    # push newly downloaded media here
