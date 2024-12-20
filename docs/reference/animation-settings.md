---
description: REFERENCE
---

import LinearEasingScreenshot from '/img/reference/animation-settings/linear-easing.png';
import BackEaseInScreenshot from '/img/reference/animation-settings/back-ease-in.png';
import BackEaseInOutScreenshot from '/img/reference/animation-settings/back-ease-in-out.png';
import BackEaseOutScreenshot from '/img/reference/animation-settings/back-ease-out.png';
import BounceEaseInScreenshot from '/img/reference/animation-settings/bounce-ease-in.png';
import BounceEaseInOutScreenshot from '/img/reference/animation-settings/bounce-ease-in-out.png';
import BounceEaseOutScreenshot from '/img/reference/animation-settings/bounce-ease-out.png';
import CircularEaseInScreenshot from '/img/reference/animation-settings/circular-ease-in.png';
import CircularEaseInOutScreenshot from '/img/reference/animation-settings/circular-ease-in-out.png';
import CircularEaseOutScreenshot from '/img/reference/animation-settings/circular-ease-out.png';
import CubicEaseInScreenshot from '/img/reference/animation-settings/cubic-ease-in.png';
import CubicEaseInOutScreenshot from '/img/reference/animation-settings/cubic-ease-in-out.png';
import CubicEaseOutScreenshot from '/img/reference/animation-settings/cubic-ease-out.png';
import ElasticEaseInScreenshot from '/img/reference/animation-settings/elastic-ease-in.png';
import ElasticEaseInOutScreenshot from '/img/reference/animation-settings/elastic-ease-in-out.png';
import ElasticEaseOutScreenshot from '/img/reference/animation-settings/elastic-ease-out.png';
import ExponentialEaseInScreenshot from '/img/reference/animation-settings/exponential-ease-in.png';
import ExponentialEaseInOutScreenshot from '/img/reference/animation-settings/exponential-ease-in-out.png';
import ExponentialEaseOutScreenshot from '/img/reference/animation-settings/exponential-ease-out.png';
import QuadraticEaseInScreenshot from '/img/reference/animation-settings/quadratic-ease-in.png';
import QuadraticEaseInOutScreenshot from '/img/reference/animation-settings/quadratic-ease-in-out.png';
import QuadraticEaseOutScreenshot from '/img/reference/animation-settings/quadratic-ease-out.png';
import QuarticEaseInScreenshot from '/img/reference/animation-settings/quartic-ease-in.png';
import QuarticEaseInOutScreenshot from '/img/reference/animation-settings/quartic-ease-in-out.png';
import QuarticEaseOutScreenshot from '/img/reference/animation-settings/quartic-ease-out.png';
import QuinticEaseInScreenshot from '/img/reference/animation-settings/quintic-ease-in.png';
import QuinticEaseInOutScreenshot from '/img/reference/animation-settings/quintic-ease-in-out.png';
import QuinticEaseOutScreenshot from '/img/reference/animation-settings/quintic-ease-out.png';
import SineEaseInScreenshot from '/img/reference/animation-settings/sine-ease-in.png';
import SineEaseInOutScreenshot from '/img/reference/animation-settings/sine-ease-in-out.png';
import SineEaseOutScreenshot from '/img/reference/animation-settings/sine-ease-out.png';

# Animation Settings

This section describes how `Animation` playback can be customized.

## Easing Functions

`Easing` functions describe how quickly an animated property changes from its starting value into its ending value across the animation time. `Avalonia.Animation.Easings` contains the following easings:

| Default                                                       |
|---------------------------------------------------------------|
| `LinearEasing`<br/><img src={LinearEasingScreenshot} alt=""/> |

| Ease-In                                                                 | Ease-Out                                                                  | Ease-In-Out                                                                   |
|-------------------------------------------------------------------------|---------------------------------------------------------------------------|-------------------------------------------------------------------------------|
| `SineEaseIn`<br/><img src={SineEaseInScreenshot} alt=""/>               | `SineEaseOut`<br/><img src={SineEaseOutScreenshot} alt=""/>               | `SineEaseInOut`<br/><img src={SineEaseInOutScreenshot} alt=""/>               |
| `QuadraticEaseIn`<br/><img src={QuadraticEaseInScreenshot} alt=""/>     | `QuadraticEaseOut`<br/><img src={QuadraticEaseOutScreenshot} alt=""/>     | `QuadraticEaseInOut`<br/><img src={QuadraticEaseInOutScreenshot} alt=""/>     |
| `CubicEaseIn`<br/><img src={CubicEaseInScreenshot} alt=""/>             | `CubicEaseOut`<br/><img src={CubicEaseOutScreenshot} alt=""/>             | `CubicEaseInOut`<br/><img src={CubicEaseInOutScreenshot} alt=""/>             |
| `QuarticEaseIn`<br/><img src={QuarticEaseInScreenshot} alt=""/>         | `QuarticEaseOut`<br/><img src={QuarticEaseOutScreenshot} alt=""/>         | `QuarticEaseInOut`<br/><img src={QuarticEaseInOutScreenshot} alt=""/>         |
| `QuinticEaseIn`<br/><img src={QuinticEaseInScreenshot} alt=""/>         | `QuinticEaseOut`<br/><img src={QuinticEaseOutScreenshot} alt=""/>         | `QuinticEaseInOut`<br/><img src={QuinticEaseInOutScreenshot} alt=""/>         |
| `ExponentialEaseIn`<br/><img src={ExponentialEaseInScreenshot} alt=""/> | `ExponentialEaseOut`<br/><img src={ExponentialEaseOutScreenshot} alt=""/> | `ExponentialEaseInOut`<br/><img src={ExponentialEaseInOutScreenshot} alt=""/> |
| `CircularEaseIn`<br/><img src={CircularEaseInScreenshot} alt=""/>       | `CircularEaseOut`<br/><img src={CircularEaseOutScreenshot} alt=""/>       | `CircularEaseInOut`<br/><img src={CircularEaseInOutScreenshot} alt=""/>       |
| `BackEaseIn`<br/><img src={BackEaseInScreenshot} alt=""/>               | `BackEaseOut`<br/><img src={BackEaseOutScreenshot} alt=""/>               | `BackEaseInOut`<br/><img src={BackEaseInOutScreenshot} alt=""/>             |
| `ElasticEaseIn`<br/><img src={ElasticEaseInScreenshot} alt=""/>         | `ElasticEaseOut`<br/><img src={ElasticEaseOutScreenshot} alt=""/>         | `ElasticEaseInOut`<br/><img src={ElasticEaseInOutScreenshot} alt=""/>         |
| `BounceEaseIn`<br/><img src={BounceEaseInScreenshot} alt=""/>           | `BounceEaseOut`<br/><img src={BounceEaseOutScreenshot} alt=""/>           | `BounceEaseInOut`<br/><img src={BounceEaseInOutScreenshot} alt=""/>           |

Additionally, you can provide your own easing by deriving from `Easing` or by providing parameters to `SplineEasing` or `SpringEasing`.

## FillModes

The `FillMode` attribute of an `Animation` defines how the animated property persists after an animation completes and during delays in-between runs.

The following table describes the supported behaviors:

| Value      | Description                                                                                               |
|------------|-----------------------------------------------------------------------------------------------------------|
| `None`     | Value will not persist after animation nor the first value will be applied when the animation is delayed. |
| `Forward`  | The last interpolated value will be persisted to the target property.                                     |
| `Backward` | The first interpolated value will be displayed on animation delay.                                        |
| `Both`     | Both `Forward` and `Backward` behaviors will be applied.                                                  |

## PlaybackDirection

`PlaybackDirection` defines how the `Animation` will be played. The following table describes the possible settings:

| Value              | Description                                             |
|--------------------|---------------------------------------------------------|
| `Normal`           | The animation is played normally.                       |
| `Reverse`          | The animation is played in reverse direction.           |
| `Alternate`        | The animation is played forwards first, then backwards. |
| `AlternateReverse` | The animation is played backwards first, then forwards. |

## IterationCount

The `IterationCount` on an `Animation` element sets how many times it is to be replayed. There are two formats for this setting:

| Value      | Description                                      |
|------------|--------------------------------------------------|
| `N`        | (N is an integer) - play N times. N can be zero. |
| `Infinite` | Repeats forever                                  |
