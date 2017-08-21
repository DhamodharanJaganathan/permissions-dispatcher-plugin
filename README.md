# PermissionsDispatcher plugin

IntelliJ plugin for supporting [PermissionsDispatcher](https://github.com/hotchemi/PermissionsDispatcher).

PermissionsDispatcher is wonderful library for Runtime Permissions. However, it asks developers "attach annotations" and "delegate to generated class" and then after that "rebuild". It's hard to follow all steps correctly. This plugin generates the skelton of methods for "attach annotations" and "delegate to generated class" using GUI.

# How to install?

Use the IDE's plugin manager to install the latest version of the plugin.

# How to use?

## Add dependencies (Optional)

* Open build.gradle and `Generate` -> `Add PermissionsDispatcher dependencies`

(If you already add the dependencies, there is no 'Add PermissionsDispatcher dependencies' menu.)

![dep](website/images/dep.gif)

## Generate Runtime Permissions codes

* Open Activity/Fragment
* `Generate` -> `Generate Runtime Permissions...`
* Choose permissions and enter method names for each annotations
* Click `Generate` button
* Done!

![pd](website/images/pd.gif)

(It skips "rebuild" for making gif small, but it is highly recommended to rebuild after generating codes.)

## Add a generation method call

* `Generate` -> `Add a generation method call`
* (If there is multiple choices, dialog asks which method you want to delegate)
* Done!

![add_delegation](website/images/add_delegation.gif)

# Settings

You can change `PermissionsDispatcher plugin` from `Preferences... > Other Settings > PermissionsDispatcher plugin`

## Rebuild

There are 3 behaviors for rebuilding project after generating PermissionsDispatcher code.

| Type             | Behavior                      |
|------------------|-------------------------------|
| Prompt (Default) | Show dialog                   |
| Always           | Always rebuild without dialog |
| Not Always       | Does not rebuild              |

# Supported PermissionsDispatcher version

* [2.1.3](https://github.com/hotchemi/PermissionsDispatcher/releases/tag/2.1.3)
* [2.2.0](https://github.com/hotchemi/PermissionsDispatcher/releases/tag/2.2.0)
* [2.2.1](https://github.com/hotchemi/PermissionsDispatcher/releases/tag/2.2.1)
* [2.3.0](https://github.com/hotchemi/PermissionsDispatcher/releases/tag/2.3.0)
* [2.3.1](https://github.com/hotchemi/PermissionsDispatcher/releases/tag/2.3.1)
* [2.3.2](https://github.com/hotchemi/PermissionsDispatcher/releases/tag/2.3.2)
* [2.4.0](https://github.com/hotchemi/PermissionsDispatcher/releases/tag/2.4.0)

## License

```
Copyright 2017 Yoshinori Isogai

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```
