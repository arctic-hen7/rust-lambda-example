# Example of Serverless Functions on Netlify in Rust

This repository is an example setup of serverless functions in Rust, using Netlify as the deployment platform.. This is a barebones playground for the serverless systems that will be integrated into [Diana](https://github.com/arctic-hen7/diana).

Unfortunately, Netlify Dev (which allows locally developing functions and the like for Netlify on your machine) does not yet support Rust serverless functions, meaning to see the results of our work, we have to deploy live to the cloud. This repository provides an example of how to do that with a basic hello world function.

Heavy inspiration for this was taken from <https://github.com/netlify/rust-functions-example>.

## To run locally

1. Fork this repository (you'll need a functioning remote) and then clone it to your local machine.
2. Run `bonnie sh` (assuming you have [Bonnie](https://github.com/arctic-hen7/bonnie) installed, if not just copy and paste the commands from `bonnie.toml`) to shell into a Docker container. This container has the same networking settings as your local machine, and all ports will be forwarded.
3. Run `netlify login` to log into your Netlify account, and then use `netlify init` to link with a repository (or you can deploy manually as per their guide).
4. Push to your remote and wait for automatic deployment!

## License

See [`LICENSE`](./LICENSE).
