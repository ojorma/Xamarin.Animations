![](Documentation/logo.png)

[![Build status](https://ci.appveyor.com/api/projects/status/8mtnmwdd4cxksy2m?svg=true)](https://ci.appveyor.com/project/aloisdeniel/xamarin-animations) 
[![NuGet](https://img.shields.io/nuget/v/Xam.Animations.svg?label=NuGet)](https://www.nuget.org/packages/Xam.Animations/) [![Donate](https://img.shields.io/badge/donate-paypal-yellow.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=ZJZKXPPGBKKAY&lc=US&item_name=GitHub&item_number=0000001&currency_code=USD&bn=PP%2dDonationsBF%3abtn_donate_SM%2egif%3aNonHosted)

This cross-platform library tends to make view animation shareable and easier for common scenarios like fade or scale entrance animations.

![](Documentation/screen.gif)

## Installation

To install Xamarin.Animations, run the following command in the Package Manager Console.

	PM> Install-Package Xam.Animations

## Usage

The package adds an `AnimateAsync` extension method to `UIView`*(iOS)* / `NSView`*(macOS)* / `View`*(Android)* / `UIElement`*(Windows)*.

To start an animation with an `IAnimation`.

```csharp
await view.AnimateAsync(Animations.FadeIn());
await view.AnimateAsync(Animations.FadeIn(duration: TimeSpan.FromSeconds(0.5f)));
await view.AnimateAsync(Animations.FadeIn(duration: TimeSpan.FromSeconds(0.5f), delay: TimeSpan.FromSeconds(0.2f)));
```

## Roadmap / ideas

* Adding WPF support

## Contributions

Contributions are welcome! If you find a bug please report it and if you want a feature please report it.

If you want to contribute code please file an issue and create a branch off of the current dev branch and file a pull request.

## License

MIT © [Aloïs Deniel](http://aloisdeniel.github.io)
