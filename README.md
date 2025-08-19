# upsnap-docker-example
Example of a docker compose file and Serve configuration for [UpSnap](https://github.com/seriousm4x/UpSnap/tree/master) that adds Tailscale connectivity as a "sidecar." Created as part of the blog post: [Make a dedicated Wake-on-LAN server with Tailscale](https://tailscale.com/blog/wake-on-lan-tailscale-upsnap).

See our [blog post on Docker](https://tailscale.com/blog/docker-tailscale-guide) or [YouTube video guide](https://www.youtube.com/watch?v=tqvvZhGrciQ) for more details and examples on configuring Tailscale inside containers.

To utilize this:
1. Create a folder on the hosting system named `upsnap`
2. Place `compose.yaml` inside the `upsnap` folder
3. Create a sub-folder inside `upsnap`, named `ts-upsnap`
4. Inside `ts-upsnap`, create folders `state` and `config`
5. If you want to access UpSnap from a single URL with no port number, as its own Tailscale node, place `upsnap.json` inside the `config` folder.
