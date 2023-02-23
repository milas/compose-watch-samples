# compose-watch-samples
Playground &amp; samples for `alpha watch` command in Docker Compose

## ReactJS
```shell
cd reactjs/
docker compose up --wait
docker compose alpha watch
```
Open http://localhost:2170 in your browser.

Modify `reactjs/src/App.js` or another source file to trigger a sync and Hot Module Reload.

Modify `reactjs/package.json` to trigger a service rebuild.
