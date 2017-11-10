# CodeClimate CLI

CodeClimate code quality SaaS (https://codeclimate.com) has it's own CLI tool that does code linting, and it's open source https://github.com/codeclimate/codeclimate.

The CLI tool uses exactly the same format as the SaaS solution, so it makes it possible to use the CodeClimate SaaS and also lint code locally.

CodeClimate CLI uses docker containers as linter engines, which makes it easy to use with Docksal.

The addon will invoke a codeclimate command reusing host docker socket. The codeclimate CLI itself will run other docker containers using same docker socket and collect data into a report.

The addon should make it possible for teams to easily add codeclimate command into their docksal commands stack.

## Installing CodeClimate addon

```bash
fin addon install codeclimate
```

## Usage

- `fin codeclimate` for a list of commands
- `fin codeclimate --no-check-version analyze -f html > codeclimate.html` to export HTML report into local directory

## More documentation

Find more documentation on official codeclimate repo:
https://github.com/codeclimate/codeclimate
