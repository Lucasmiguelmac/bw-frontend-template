# Svelte-Template

# Description
Template for developing, deploying and locally-testing Svelte-powered frontends.

# Template Roadmap
* [x] Template for SPA.
* [x] Template for Routed Frontend.
* [ ] Template for PWA.
* [ ] Enable component reuse between Web and Mobile apps.
* [ ] Enable component reuse between Web, Mobile and Desktop apps.
* [ ] Enable component reuse between Web, Mobile, Desktop and Wearable apps.
* [ ] Interactive command to start a new frontend project.
    * [ ] Choose in how many devices you want your project to live.
    * [ ] Pick a routing solution if any (else: SPA)
    * [ ] Pick unit tests config
        * [ ] Component renderer
        * [ ] Test runner (uvu, jest, ava, etc.)
        * [ ] Mocking solution
    * [ ] Toggle TS use
    * [ ] Publish as Svelteplate

## CI/CD docker commands

### Production
```sh
docker run --name svelte_template -it -p 80:80 --rm $(docker build -q -f Dockerfile.build .)
```

### Dev
```sh
docker run --name svelte_template -it -p 3000:3000 -v "$(pwd)/src:/usr/src/app/src" --rm $(docker build -q -f Dockerfile.dev .)
```
