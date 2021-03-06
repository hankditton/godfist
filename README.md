# Godfist

## Godfist is a wrapper for League of Legends' ReST API written in Elixir.

#### Don't forget to check the [documentation](https://hexdocs.pm/godfist/Godfist.html) for a complete reference to the library.

<img src="priv/godfist.png" alt="Notify" width="400" height="300" align="left" />

## Installation

First include `godfist` in your `mix.exs` and add it to your applications.

```elixir
[extra_applications: :godfist, ...]
...
{:godfist, "~> 0.2.2"}
```

You can use `{:godfist, github: "aguxez/godfist"}` for the development version.

#### Note: if a function is in the docs but not available in your package version, use Github's instead.

## Usage
Remember to set your api key on your `config.exs` with the next params.

```elixir
config :godfist,
token: "YOUR API KEY",
time: 1000, # This is the minimum default from Riot, set this time in miliseconds.
amount: 20 # Amount of request limit, default minimum is 20 each second for development.
```

Or export the api key as "RIOT_TOKEN": `export RIOT_TOKEN="token"`


#### TODO: Add tournament endpoints.
