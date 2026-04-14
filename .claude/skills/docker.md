<skill_context>
Dockerization Standards
</skill_context>
<rules>
- Use lightweight `alpine` or `-slim` based Node images.
- Enforce Multi-Stage builds (e.g. `builder` stage for deps/compilation, `runner` stage for production output).
- Ensure the Node application never runs as `root`. Drop privileges to the `node` user.
- Export ports predictably (e.g., EXPOSE 3000).
- Provide a robust `docker-compose.yml` to orchestrate Postgres and the Node/React containers locally.
</rules>