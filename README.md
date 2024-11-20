
> Open this page at GitHub Pages: [https://github.com/jp-96/amq-pxt-accelmagiq-estimator/](https://github.com/jp-96/amq-pxt-accelmagiq-estimator/)

## Quaternions with AccelMagiQ and micro:bit!

A Simplified Analytic Attitude Determination Algorithm
using Accelerometer and Magnetometer on micro:bit.

It's like magic! This algorithm turns raw data into accurate and efficient quaternion estimations,
transforming your projects and making you go, "Wow!" Using the handy micro:bit, it feels like trying
out quaternions is pure magic. AccelMagiQ brings a touch of enchantment to the technical world.
We hope this helps you in your learning journey and sparks your curiosity about the fascinating
world of quaternions.

"AccelMagiQ" refers to this amazing algorithm that combines accelerometer and magnetometer data to
create precise quaternion calculations. It's a playful blend of 'acceleration', 'magnetometer', and 'magic' with
quaternions ('Q'), making advanced concepts seem like magic!

# Blocks preview

<!--
This image shows the blocks code from the last commit in master.
This image may take a few minutes to refresh.

![A rendered view of the blocks](https://github.com/jp-96/amq-pxt-accelmagiq-estimator/raw/master/.github/makecode/blocks.png)
-->
![A rendered view of the blocks](https://github.com/jp-96/amq-pxt-accelmagiq-estimator/raw/master/.github/statics/blocks.png)

## Use as Extension

This repository can be added as an **extension** in MakeCode.

* open [https://makecode.microbit.org/](https://makecode.microbit.org/)
* click on **New Project**
* click on **Extensions** under the gearwheel menu
* search for **https://github.com/jp-96/amq-pxt-accelmagiq-estimator** and import

## Downloaded HEX file to Use as Extension

Released HEX file can be imported as an **extension** in MakeCode.

* open [https://github.com/jp-96/amq-pxt-accelmagiq-estimator/releases](https://github.com/jp-96/amq-pxt-accelmagiq-estimator/releases)
* download HEX file
* open [https://makecode.microbit.org/](https://makecode.microbit.org/)
* click on **New Project**
* click on **Extensions** under the gearwheel menu
* click on **Import File**
* select downloaded HEX file and click on **Go ahead!**

## Example

```blocks

if (input.buttonIsPressed(Button.B)) {
    input.calibrateCompass()
}
accelmagiq.setCoordinateSystem(accelmagiq.CoordinateSystem.BASIC)
accelmagiq.setLowPassFilterAlpha(0.3)
basic.forever(function () {
    accelmagiq.notifyData(accelmagiq.estimate())
})

```

```js

if (input.buttonIsPressed(Button.B)) {
    input.calibrateCompass()
}
accelmagiq.setCoordinateSystem(accelmagiq.CoordinateSystem.BASIC)
accelmagiq.setLowPassFilterAlpha(0.3)
basic.forever(function () {
    accelmagiq.notifyData(accelmagiq.estimate())
})

```

#### Metadata (used for search, rendering)

* for PXT/microbit

<script src="https://cdn.jsdelivr.net/gh/jp-rad/pxt-ubit-extension@0.5.0/.github/statics/gh-pages-embed.js"></script>
<script>makeCodeRender("{{ site.makecode.home_url }}", [ "custom=github:jp-96/amq-pxt-accelmagiq-estimator", ]);</script>
