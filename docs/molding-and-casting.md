---
title: Molding and Casting
has_children: false
nav_order: 1
layout: default
---

# Molding and Casting for Soft Robotics
{: .no_toc }
Soft robots tend to rely on internal structures to operate. The infamous [PneuNets actuator](//softroboticstoolkit.com/book/pneunets-bending-actuator) used in many different soft robotic designs rely on a set of internal bellows that expand. Soft robotic sensors, especially those that operate using fluids like [salt water](//softroboticstoolkit.com/contact-sensor) or [EGaIn](//softroboticstoolkit.com/book/egain-sensors), rely on fluid channels that change shape and volume. The most common design element amongst these robotic components is usually silicone elastomer. Silicone rubber, unlike metal and most plastics, can stretch and deform by over 600% their original shape. Silicone rubber is also soft and compliant, like human tissue, so it is safer to be used around humans.

However, the main disadvantage of silicone rubber is that it is so compliant that traditional machining or manufacturing to achieve highly complex shapes is not feasible. This is why **molding and casting** silicone rubber is usually the preferred method for making soft robots.

Here, we present a brief overview and some guidelines on how to make soft robots with molding and casting. This guide also serves as a precursor to the concepts presented in the paper for those who are not familiar with soft robotic fabrication.

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Fabrication Concepts
### Casting
**Casting** is the act of pouring or injecting a material in its liquid state into a cavity that resembles the final product. The liquid material will then solidify in the cavity or **mold** and then the mold is either removed or destroyed - leaving just the finished part. For soft robots, typically this liquid is the silicone rubber in its uncured state, which is usually a mixture of Part A and Part B of the silicone rubber.

### Molding
Molding and casting go hand-in-hand. Molding is the act of the making the cavity or mold where you would inject or pour the material to be casted. For the [special effects industry](//www.youtube.com/watch?v=DEVi0mEaJJQ), these molds are usually made by casting themselves, which usually involves casting around a "master" prop in a box to get a mold. For soft robotics purposes, we would desire a more repeatable process, so most molds in soft robotics research is 3D printed. With a highly-detailed mold, the liquid silicone rubber usually picks up all the fine details once casted so any external features can be simply designed into the 3D printed mold.

There are many types of molds depending on the technique used in casting, that are used in the industry. The simplest mold is an open-top mold where the material can be simply poured into a "tub" that resembles the end product shape - this type of mold has limited use since one side of the finished product must be flat. Another type of mold is *injection molding*. Injection molding can be attributed to also plastics and metal injection molding, where high pressure and high temperature material is injected into a mold. Plastic injection molding is industry standard to make almost every piece of plastic you can find in everyday life. For silicone rubbers, however, injection molding refers to injecting liquid silicone rubber into a closed mold, with only an opening for the injection port.

### Cores
External features can be created with molds, but what about internal features? In metal casting, for example to cast an engine, a **core** must be used to create the internal cavity for the pistons. Cores cannot be made out of solid material since they need to be removed later, so engine manufacturers usually use sand and binder to make temporary cores that are removed after the molten metal cools down and solidifies. For jewelers, lost-wax casting or investment casting is usually preferred. Wax can be 3D printed to make the core and later burned out after casting.

For soft robots, the core usually makes up the internal features of the components, such as a bladder or fluid channel. Wax can be used to make soft robot cores, but wax is prone to dimensional inaccuracies by shrinkage and is very fragile. Wax also requires being melted out, which depending on the wax can leave unwanted residue on the internal surface. Some internal features can be made by casting two or more separate pieces of the soft robotic component and later bond them together, but this requires multiple steps and the bonding can fail.

Our paper introduces two new concepts to soft robotic fabrication: 3D printed [sacrificial](/negshell-cores) and [structural cores](/structural-cores) that are designed to be *left in* the soft robotic component rather than being removed after casting.

## Materials and Equipment
The following is a non-exhaustive list of materials and equipment for fabricating silicone-rubber based soft robots
### Silicone Rubber
Silicone rubber usually comes in two different chemistries: Platinum-Cure and Tin-Cure. Each have their own pros and cons. Silicone rubber is also generally categorized by how **soft** they are (the durometer) using the Shore scale. Starting from Shore 00-0 to Shore 00-40, which as soft as a gummy bear, to Shore 10A to Shore 80A which ranges from a rubber band to a hard eraser. Higher durometer in the Shore 30D to Shore 100D elastomers are typically urethane or plastic, not silicone.
#### Platinum-Cure Silicone
The platinum in Platinum-Cure silicone refers to the catalyst used to start the cure or hardening process. Platinum-cure silicone is known to be sensitive to any contaminants, which can inhibit curing. However, platinum-cure silicone has better overall mechanical properties and uncured shelf-life. Preparing platinum-cure silicone usually requires a 1-to-1 mixing ratio, making it less susceptible to measuring errors. Some platinum-cure silicone is also skin-safe and can be used for making food.

Example platinum-cure silicones available to purchase

|Name|Durometer|Link|
|----|---------|----|
|Plat-Sil Gel 10|10A|[Polytek](//www.polytek.com/products/platsil-gel-10)|
|**Plat-Sil Gel 25**|25A|[Polytek](//www.polytek.com/products/platsil-gel-25)|
|Dragon Skin 30|30A|[Smooth-on](//www.smooth-on.com/products/dragon-skin-30/)|
|Smooth-Sil 945|45A|[Smooth-on](//www.smooth-on.com/products/smooth-sil-945/)|

The authors generally prefer **Plat-Sil Gel 25** due to its translucency, 1 hour demold time and biocompatibility. The same silicone rubber is used throughout the paper.

#### Tin-Cure Silicone
Tin-cure silicone or condensation cure silicone are not so great.
#### Silicone Adhesives


### Release Agents

### Vacuum Degassing

## Guidelines
