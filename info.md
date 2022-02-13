# Hacky support for STYJ02YM/STYTJ02YM
This hacky integration adds support for Xiaomi Robot Vacuum-Mop Pro, Viomi V2 Pro and other devices widely known as STYTJ02YM.  
Repository was forked from https://github.com/nqkdev/home-assistant-vacuum-styj02ym, by KrzysztofHajdamowicz whos backported changes from other forks, added HACS compatibility and polished it a bit.  
Then I forked it in order to merge support for china version of the vacuum from other forks, and updated code base in order to fix warnings.

## Installation:
- install it with HACS
- Add the configuration to configuration.yaml, example:

### Usage

Add to `configuration.yaml`:

```yaml
vacuum:
  - platform: miio2
    host: 192.168.1.xxx
    token: !secret vacuum
    name: vacuum_name
    china_version: False
```
