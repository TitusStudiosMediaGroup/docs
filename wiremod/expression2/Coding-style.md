In general, just follow the [Lua style guide](http://lua-users.org/wiki/LuaStyleGuide).

The Wiremod Code Style Guide takes precedence in case of disagreement.

## Naming

* Constants (whether local or global) should be named in `UNDERSCORED_UPPERCASE`.
* Locals (whether file scope, arguments or otherwise) should be named in `dromedaryCamelCase`.
* Globals and fields should be named in `BactrianCamelCase`.
* Files should be named in `underscored_lowercase.lua`. Unless your code is for an entity, weapon or effect, it should be in `lua/wire/client/`, `lua/wire/server/`, or `lua/wire/` (for shared code). If related code will span multiple files then it should probably be in its own subdirectory in one of these.

## Spacing

To make sure the code is readable with all tab sizes, we use tabs for indentation and spaces for alignment.

Your code shouldn't have trailing whitespace, and your editor should be configured to either do no cleanup or to follow this code style guide in order to avoid making your diff messy. The diff should only touch the code that's actually relevant.

Files should end with a newline character.

There should be spaces after commas, around operators and inside `{` curly braces `}`, but not inside `(`parentheses`)` or `[`square brackets`]`.

## Other stuff

* Non-standard language elements like C-style operators (eg. `!`, `&&`), C-style comments (`//`) and `continue` are banned. They're a custom feature of Garry's Mod Lua and usually unsupported in other environments.
* No parentheses around if conditions.
* Do not omit parentheses around function arguments.
* Most of these rules can be ignored in special DSL constructs.

## Non-code stuff

* Code that goes into wire proper cannot favor specific addons not managed by the [@wiremod](https://github.com/wiremod) organization. Adding hooks/callbacks/interfaces to support external addons is fine. Code in the [`wire-extras`](https://github.com/wiremod/wire-extras) repository is specifically exempt from following this rule.