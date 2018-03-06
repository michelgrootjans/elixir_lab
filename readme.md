To run elixir:
> docker-compose run lab

mix new lab
cd lab
mix test

# mix.exs
def deps do
  [
    ...
    {:mix_test_watch, "~> 0.5", only: :dev, runtime: false}
    ...
  ]  
end