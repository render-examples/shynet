# Deploy Shynet on Render

This repo can be used to deploy [Shynet] on Render.

- It uses the [official Shynet Docker image](https://hub.docker.com/r/milesmcc/shynet).
- [Render Databases](https://render.com/docs/databases) are used to spin up a fully managed PostgreSQL instance.

## Deployment

### One Click Deploy

Use the button below to deploy Shynet on Render.

[![Deploy to Render](http://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy)

After deployment, use Render **Shell** to set up your Shynet account:

1. Set your email with `./manage.py registeradmin your-email@example.com`. You will be prompted with a temporary password. Save it.
2. Set your whitelabel with `./manage.py whitelabel "Header for your Shynet site"`. It will be shown at the top of your Shynet site.

 Also use the service **Environment** page to update the `CSRF_TRUSTED_ORIGINS` environment variable to your deployed Render service domain.

### Manual Deployment

See the guide at https://docs.render.com/deploy-shynet

[shynet]: https://github.com/milesmcc/shynet
