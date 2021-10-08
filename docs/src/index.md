# FerriteVis.jl

FerriteVis.jl is a small package to visualize your Ferrite.jl results. Currently all Makie backends are supported and thus,
you can visualize your results in a GLMakie window, inside Pluto/Jupyter notebooks via WGLMakie and produce nice vector graphics with
CairoMakie.

In the future this package tries to adapt also other plotting packages, such as Plots.jl and PGFPlotsX.jl. Contributions are highly welcome.

## Getting Started

Install FerriteVis.jl with the in-built package manager of Julia

```julia
pkg> add FerriteVis
```

Do your computation with Ferrite.jl and save the used `DofHandler` and solution vector into a variable. Pass those two variables into
the `MakiePlotter` constructor

```julia
plotter = MakiePlotter(dh,u)
```

Now, you can use all common Makie plotting functionalities, such as `mesh`, `surface` and `arrows`. For a more detailed example, check out the tutorial page.