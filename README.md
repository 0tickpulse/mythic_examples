# Mythic Examples

A comprehensive list of examples of configurations in the Mythic plugin.

## Contributing

You are welcome to contribute to this repository. However, there are a few conditions:

1. Your configuration must be thoroughly and fully tested.
1. Usage has to be clearly documented.
1. Configuration must be drop-in ready unless specified otherwise.

### Color codes

**Always use Minimessage unless necessary**. An example of a script that requires legacy color codes:

```yaml
ColorSkill:
  Skills:
    - message{m=&<random.0to9>Random color!} @Self
```

### File structure

Files are structured in this way: Following the root of the repository, there are packs of mythic configurations.
