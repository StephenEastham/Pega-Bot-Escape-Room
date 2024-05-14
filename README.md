# Pega Bot

This set of software components extends Pega low-code (in Agile Studio) with the ability to control a lego robot and other items, such as a camera.

There are three major components:

## BotController Bridge
This component acts as a bridge to transfer instructions between an Internet-connected laptop (or other device) and the lego robot hub. The bridge transfers the instructions: either from the device to the hub, first over HTTP and then via BLE  ; or from the hub to the device, first via BLE and then over HTTP.

## BotController Camera Embedded
This component runs on a Raspberry Pi device with a camera, and therefore allows Pega low-code to take photos. The device requires an Internet connection to work.

## BotController Spike Prime Embedded
This component uses pybricks to control a lego robot that is based on a SPIKE Prime multi-port Hub. To use pybricks, you must first flash pybricks to the Hub.

