# Nuxt + Netlify + Contentful Demo

- Nuxt
  - "The Vue.js Framework"
- Netlify
  - "Build, deploy, and manage modern web projects"
  - "Static without limits"
- Contentful
  - "Manage content better with infrastructure"
  - "The cure for the common CMS"

1. Setup Nuxt
   - [x] Install `nuxt`
   - [x] Add `dev` script
   - [x] Create `pages` and setup links
   - [x] Create `nav` component
       - [x] Demo `<script>` and `<style>`
       - [x] Create links manually in template
       - [x] Add `links` prop with default
       - [x] Demo `v-for` and `v-text` bind directives
   - [x] Demo Vue dev tools
   - [x] Create `default` layout
       - [x] Add some padding
   - [x] Demo `universal` mode with SSR
   - [x] Add `build` and `start` scripts
   - [x] Demo `build --analyse`
   - [x] Demo SPA mode
       - [x] CLI `--spa` flag
       - [x] `nuxt.config.js`
   - [x] Install `normalize.css` and add global styles
       - [x] html font-size, font-family
   - [x] Demo `generate` static site
   - [x] Install `serve` and create respective script
   - [x] Revert to universal mode (remove `mode` from config)
   - [x] Configure generate `subFolders`
   - [x] Demo `--modern=client`
   - [x] Nuxt is very versatile!
2. Deploy to Netlify
   - [x] Drag and drop
   - [x] Review site with network tools
       - [x] HTTPS + HTTP2 by default
   - [x] Change site name
   - [x] Make some obvious changes
       - [x] html min-height, background-color
       - [x] Demo `<style>` in nav component
       - [x] Switch to SASS
       - [x] Install (`node-sass`, `sass-loader`)
   - [x] Drag and drop again
   - [x] Preview previous deploy
   - [x] Rollback version
3. Version control integration
   - [x] Create `.gitignore` and `git init`
   - [ ] Push project to GitHub
   - [ ] Link GitHub repo to Netlify
   - [ ] Configure `command` and `publish` in Netlify UI
   - [ ] Review live deploy logs (CD first run)
   - [ ] Make another change in `master`
       - [ ] Add broken link to nav
       - [ ] Push to GitHub
   - [ ] Review deploys
   - [ ] Navigate to broken link
   - [ ] Create a new branch `feat/error-page`
       - [ ] Create `error` layout
       - [ ] Create `blank` layout
   - [ ] Push to GitHub
4. Continuous deployment
   - [ ] Review deploys (no deployment for feature branch)
   - [ ] Create pull request
   - [ ] Review deploys
   - [ ] Demo Netlify integration in PR
       - [ ] Click broken link—works
       - [ ] Refresh: page not found
       - [ ] Config `generate.fallback: true`
   - [ ] Merge into master
   - [ ] Review deploys
   - [ ] Setup branch deploys
   - [ ] Create another branch
   - [ ] Make obvious change (background-color)
   - [ ] Push to GitHub
   - [ ] Review deploys
5. Split testing
   - [ ] Start split test + refresh
   - [ ] Netlify build node env vars + Google Analytics (`BRANCH`)
   - [ ] Stop split test + refresh
6. Setup Contentful
   - [ ] Create a space (NCC)
   - [ ] Create a content model (film)
       - [ ] Name (required)
       - [ ] Slug (required, unique)
       - [ ] Cover (required, image)
       - [ ] Release Date (required, format)
       - [ ] Rating (min, max, appearance)
7. Author some content
   - [ ] Create a few entries
   - [ ] Review media tab
   - [ ] Publish a couple of entries
8. Integrate Contentful
   - [ ] Install contentful SDK
   - [ ] Create CMS plugin
   - [ ] Create API key and copy
       - [ ] Space ID
       - [ ] CDA token
       - [ ] CPA token
   - [ ] Render entries on list page
   - [ ] Demo preview API
   - [ ] Demo Image API (w, h, fit, format)
   - [ ] Create dynamic page
   - [ ] Generate static site...no film pages
   - [ ] Setup generate `routes` in Nuxt config (fallback, subFolders)
   - [ ] Setup asyncData `payload`
9. Setup webhooks
   - [ ] Netlify > Settings > Build & deploy > Build hooks (`master`)
   - [ ] Contentful `?trigger_title=Deploy+triggered+by+Contentful`
   - [ ] Edit and save some published content
   - [ ] Review Netlify deploys
   - [ ] Create `preview` branch
   - [ ] Create `netlify.toml`
       - [ ] `build` settings
       - [ ] Branch env vars
