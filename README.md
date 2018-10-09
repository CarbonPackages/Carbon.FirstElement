[![Latest Stable Version](https://poser.pugx.org/carbon/firstelement/v/stable)](https://packagist.org/packages/carbon/firstelement)
[![Total Downloads](https://poser.pugx.org/carbon/firstelement/downloads)](https://packagist.org/packages/carbon/firstelement)
[![License](https://poser.pugx.org/carbon/firstelement/license)](LICENSE)
[![GitHub forks](https://img.shields.io/github/forks/CarbonPackages/Carbon.FirstElement.svg?style=social&label=Fork)](https://github.com/CarbonPackages/Carbon.FirstElement/fork)
[![GitHub stars](https://img.shields.io/github/stars/CarbonPackages/Carbon.FirstElement.svg?style=social&label=Stars)](https://github.com/CarbonPackages/Carbon.FirstElement/stargazers)
[![GitHub watchers](https://img.shields.io/github/watchers/CarbonPackages/Carbon.FirstElement.svg?style=social&label=Watch)](https://github.com/CarbonPackages/Carbon.FirstElement/subscription)

# Carbon.FirstElement Package for Neos CMS

Get a boolean value returned if a content element is the first element in a ContentCollection or not. Great for automated headlines (`h1` or `h2`)

## Installation

`Carbon.FirstElement` is available via packagist. Add `"carbon/firstelement" : "^1.0"`
to the require section of your composer.json or run `composer require carbon/firstelement`.

## Usage

If you add the super type `Carbon.FirstElement:Mixin` to a node type definition, you activate the FlowQuery in the prototype `Carbon.FirstElement:Mixin`. Every `Neos.Neos:Content` and `Neos.Neos:ContentComponent` get automatically the property `isFirstElement`. If you want to extend another prototype you can do it like this:

```elm
prototype(Your.Package:Content) {
    isFirstElement = Carbon.FirstElement:Mixin
}
```

## License

Licensed under MIT, see [LICENSE](LICENSE)
