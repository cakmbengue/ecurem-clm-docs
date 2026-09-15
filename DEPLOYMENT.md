# Deployment

Production document root:

    /var/www/docs.ecurem.cloud/public

Recommended deployment model:

1. validate the Git commit locally;
2. create a backup of the current production `public/` tree;
3. copy the repository `public/` contents to the production document root;
4. restore `root:www-data` ownership;
5. set directories to 750 and files to 640;
6. run `nginx -t`;
7. reload Nginx only after a successful configuration test;
8. test `/`, `/en/`, `/security/`, `/discovery/`, `/renewal/` and static assets.

The production web process should not have write access to published documentation.
