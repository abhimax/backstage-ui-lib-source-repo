# Backstage Integration

This directory is a placeholder for Backstage-related configuration or documentation.

## How to use this project with Backstage

1. Register this project in your Backstage instance by adding the `catalog-info.yaml` file to your Backstage catalog.
2. Update the `owner` and `github.com/project-slug` fields in `catalog-info.yaml` as appropriate for your organization.
3. Use this project as a component or library in your Backstage ecosystem.

## Documentation in Backstage

This project includes sample documentation files in the `docs/` directory. You can use the Backstage TechDocs plugin to render these markdown files as documentation in your Backstage instance.

### TechDocs Setup

The project is configured to use the **local generator** instead of Docker. This means:

1. **No Docker required** - TechDocs will use local Python/MkDocs installation
2. **Faster builds** - No container overhead
3. **Easier debugging** - Direct access to build logs

### Troubleshooting TechDocs

If you encounter issues:

1. **Docker errors**: The project is configured to use local generator (`backstage.io/techdocs-generator: local`)
2. **Missing dependencies**: Install MkDocs and TechDocs plugins:
   ```bash
   pip install mkdocs mkdocs-techdocs-core
   ```
3. **Build failures**: Check the `mkdocs.yml` configuration and ensure all markdown files exist

See the `docs/README.md` for more details about the documentation structure. 