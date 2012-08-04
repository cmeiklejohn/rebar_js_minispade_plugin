# Rebar JS Minispade Plugin

Minispade support during rebar compilation.

## Installation

Specify ```rebar_js_minispade_plugin``` as a dependency in your ```rebar.config```.

```erlang
{deps, [
       {rebar_js_minispade_plugin, ".*",
        {git, "git://github.com/cmeiklejohn/rebar_js_minispade_plugin.git", {branch, "master"}}}
]}.
```

Then, configure as a plugin in your ```rebar.config```.

```erlang
{plugins, [rebar_js_minispade_plugin]}.
```

## Configuration

Example usage:

```erlang
{js_minispade, [
    {out_dir,  "priv/assets/javascripts"},
    {doc_root, "priv/www/javascripts"},
    {modules,  ["models", "controllers"]}
]}.
```
