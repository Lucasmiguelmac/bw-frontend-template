# Svelte-Template

# Description
Template for developing, deploying and locally-testing Svelte-powered frontends.

# Template Roadmap
* [ ] Template for SPA.
* [ ] Template for Routed Frontend.
* [ ] Enable component reuse between Web and Mobile apps.
* [ ] Enable component reuse between Web, Mobile and Wearable apps.


## CI/CD docker commands

### Production
```docker run --name svelte_template -it -p 80:80 --rm $(docker build -q -f Dockerfile.build .)```

### Dev
```docker run --name svelte_template -it -p 3000:3000 -v "$(pwd)/src:/usr/src/app/src" --rm $(docker build -q -f Dockerfile.dev .)```
