# RestPortal

The main question that comes to mind while designing a full stack applications, How to reliably automate the build/test of our precious code and deploy it into production. While it's impossible to create ultimate solution that runs like a breeze, we can still get a robust bulid pipeline using simple workflow.

Our build pipeline should do the following:
- Carry out fast deployment
- Require minimum manual intervention
- Handle deployment into different namespaces

## Helm commands
```sh
helm install -f values.yaml --name dev backend
helm --debug upgrade --install dev backend
helm ls --all dev
helm del --purge dev
```
