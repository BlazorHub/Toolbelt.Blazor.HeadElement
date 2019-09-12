# Blazor Head Element Helper [![NuGet Package](https://img.shields.io/nuget/v/Toolbelt.Blazor.HeadElement.svg)](https://www.nuget.org/packages/Toolbelt.Blazor.HeadElement/)

## Summary

This component and services allows you to **change the title of document on your Blazor app**.

This package supports both of seiver-side Blazor and client-side Blazor WebAssembly app.

And also supports server-side pre-rendering on your server-side Blazor app.

### NOTICE! - This is "Preview" Release

This package is **"preview" release** at this time.

Some implementations of this packages depends on internals of ASP.NET Core Components.

Especially, server-side pre-rendering is very slow and stressfull, because **it captures all requests and buffering all responses on memory.**

## How to use

1. Add package to your project like this.

```shell
dotnet add package Toolbelt.Blazor.HeadElement --version 0.0.1-preview1.0.1
```

2. Open `Toolbelt.Blazor.HeadElement` namespace.

```
@* This is "_Imports.razor" *@
...
@using Toolbelt.Blazor.HeadElement
```

3. Markup `<Title>` component in your .razor file.

```html
@* This is "Pages/Counter.razor" *@
@page "/counter"

<Title>Counter(@currentCount) - Server Side App</Title>
```

The title of document will be changed.

![fig1](https://raw.githubusercontent.com/jsakamoto/Toolbelt.Blazor.HeadElement/master/.assets/fig1.png)

## License

[Mozilla Public License Version 2.0](https://raw.githubusercontent.com/jsakamoto/Toolbelt.Blazor.HeadElement/master/LICENSE)
