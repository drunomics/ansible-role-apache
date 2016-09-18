#drunomics.apache
Ansible role that installs apache.

## Configuration

- See defaults/main.yml for supported configuration options.
- See tests/test-*.yml test playbooks for examples.

## Adding password protection

1. Configure a suiting htpasswd file that contains allowed users

```
apache_htpasswd_files:
  default:
   - "user:$apr1$v9CvCAag$Ow.1dk44cqh5cd87FYE6M1"
```
The lines can be created as follows:
```
htpasswd -n testuser
# Prompt for entering the password follows.
```

## Support
Distribution: Ubuntu

Supported releases:
- 12.04
- 14.04 (tested)
- 16.04 soon 


(c) 2016 drunomics GmbH. /  MIT License
