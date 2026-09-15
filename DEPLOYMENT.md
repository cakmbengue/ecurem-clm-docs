# Deployment

The deployable static site is located under `public/`.

Recommended deployment model:

1. validate the Git commit locally;
2. create a backup of the currently published documentation;
3. deploy the repository `public/` contents to the production web root;
4. restore the expected ownership and permissions;
5. validate the Nginx configuration;
6. reload Nginx only after a successful configuration test;
7. test the French and English documentation routes and static assets.

The production web process should not have write access to published documentation.

Infrastructure-specific paths, credentials and internal deployment details are intentionally not documented in this public repository.
