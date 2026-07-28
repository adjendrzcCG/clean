# GenRevive Clean Modernization Template

Welcome to your clean modernization workspace! This template provides a structured environment for application modernization using GenRevive.

## Overview

This workspace is preconfigured with:
- **Development Container** - Consistent development environment
- **Modernization Configuration** - Core settings for your migration
- **Setup Scripts** - Initialization and automation tools
- **Documentation** - Guidelines and best practices

## Getting Started

### 1. Initialize Your Workspace
```bash
bash scripts/init.sh
```

This script will:
- Install dependencies
- Configure Git hooks
- Set up local environment variables
- Initialize modernization tracking

### 2. Review Configuration
Edit `config/modernization-config.json` with your project details:
```json
{
  "projectName": "Your Application Name",
  "targetPlatform": "Azure",
  "estimatedComplexity": "medium",
  "stakeholders": ["team@company.com"]
}
```

### 3. Access GenRevive Platform
- Navigate to: https://genrevive-cockpit.azurewebsites.net
- Link this codespace repository in your portfolio
- Begin the modernization workflow

## Project Structure

```
.
├── config/                  # Configuration files
│   └── modernization-config.json
├── scripts/                 # Utility scripts
│   ├── init.sh            # Initialize workspace
│   └── setup.sh           # Development setup
├── .devcontainer/         # Container configuration
│   └── devcontainer.json
├── docs/                  # Documentation
│   └── GETTING_STARTED.md
└── README.md             # This file
```

## Next Steps

1. **Configure Your Project**: Update `config/modernization-config.json`
2. **Initialize**: Run `bash scripts/init.sh`
3. **Explore**: Review modernization options in GenRevive
4. **Execute**: Follow the generated migration plan

## Support

For questions or issues:
- Check [GenRevive Documentation](https://github.com/genrevive/docs)
- Review modernization best practices in `/docs/`
- Contact your modernization team

## Troubleshooting

### Setup fails
- Ensure Docker/Podman is running for devcontainer
- Run scripts with `bash` to avoid execute-bit issues after template upload: `bash scripts/init.sh`, `bash scripts/setup.sh`
- Optional: restore execute permissions if you prefer `./scripts/...`: `chmod +x scripts/*.sh`

### Configuration errors
- Validate JSON in `config/modernization-config.json`
- Ensure all required fields are populated

### Still need help?
Contact: modernization-support@genrevive.io

---

**Generated**: $(date)  
**Template Version**: 1.0  
**GenRevive Platform**: v1.16.0
