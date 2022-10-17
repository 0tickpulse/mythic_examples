# Mythic Examples

A comprehensive list of examples of configurations in the Mythic plugin.

## Contributing

You are welcome to contribute to this repository. However, there are a few conditions:

1. Your configuration must be thoroughly and fully tested.
1. You must follow the proper code style.
1. Be clearly documented.
1. Configuration must be drop-in ready unless specified otherwise.

### Code style and file structure

#### Casing

| Token type                          | Casing method |
| ----------------------------------- | ------------- |
| AITargetSelector/AIGoalSelector IDs | `camelCase`   |
| Mechanic IDs                        | `camelCase`   |
| Skill attribute names               | `camelCase`   |
| Trigger IDs                         | `camelCase`   |
| Filenames                           | `PascalCase`  |
| Meta-skill IDs                      | `PascalCase`  |
| Pack IDs                            | `PascalCase`  |
| Targeter IDs                        | `PascalCase`  |
| Disguise entity IDs                 | `MACRO_CASE`  |

For example:

```yaml
# Bad!
someSkill:
  Skills:
    - Message{m=Hello} @self
```

```yaml
# Good!
SomeSkill:
  Skills:
    - message{m=Hello} @Self
```

#### Indentation of YAML

Always use 2-space indentation. In addition, lists have to have an extra indentation.

```yaml
# Bad!
Somelist:
- 1
- 2
- 3
```

```yaml
# Good!
Somelist:
  - 1
  - 2
  - 3
```

#### Color codes

**Always use Minimessage unless necessary**. An example of a script that requires legacy color codes:

```yaml
ColorSkill:
  Skills:
    - message{m=&<random.0to9>Random color!} @Self
```

#### File structure

Files are structured in this way: Following the root of the repository, there are packs of mythic configurations.
