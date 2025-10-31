# macos_ansible
macos initial setup with ansible

## Usage

Run the playbook with:
```bash
ansible-playbook macos.ansible.yml --ask-become-pass
```

Note: This needs full disk access and permissions for Terminal to modify system settings.

## Creating a Release

To create a new release:

1. Create and push a version tag:
   ```bash
   git tag v1.0.0
   git push origin v1.0.0
   ```

2. The GitHub Actions workflow will automatically:
   - Create a new GitHub release
   - Generate release notes from commit history
   - Publish the release

Version tags should follow semantic versioning (e.g., v1.0.0, v1.2.3, v2.0.0)
