---
title: "ContourLayer Class | Microsoft Docs"
ms.custom: ""
ms.date: "02/28/2018"
ms.reviewer: ""
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "article"
ms.assetid: b7032c94-f447-4bdb-be13-55f289dea12b
caps.latest.revision: 5
author: "rbrundritt"
ms.author: "richbrun"
manager: "stevelom"
---
# ContourLayer Class
The ContourLayer class takes an array of [ContourLine](../v8-web-control/contourline-class.md) and organizes them and creates non-overlapping polygon to represent each contour area.

## Constructor

> ContourLayer(contourLines: [ContourLine](../v8-web-control/contourline-class.md)\[\], options?: [ContourLayerOptions](../v8-web-control/contourlayeroptions-object.md))

## Methods


| Name                                           | Return Type         | Description                                                                 |
|------------------------------------------------|---------------------|-----------------------------------------------------------------------------|
| `clear()`                                        |                     | Clears all data on the contour layer.                                       |
| `getContourLines()`                              | [ContourLine](../v8-web-control/contourline-class.md)\[\]     | Gets the contour lines of this layer.                                       |
| `getContourPolygons()`                             | [Polygon](Polygon%20Class.md)\[\]         | Gets the polygons that were generated from the contour lines in this layer. |
| `getOptions()`                                  | [ContourLayerOptions](../v8-web-control/contourlayeroptions-object.md) | Retrieves the options of this contour layer.                                |
| `getVisible()` | boolean |Gets a boolean that indicates if the layer is visible or not. | 
| `getZIndex()` | number | Gets the zIndex of the layer. | 
| setContourLines(contourLines: [ContourLine](../v8-web-control/contourline-class.md)\[\]) |                     | Sets the contour lines used to calculate the polygon areas of this layer.   |
| setOptions(options: [ContourLayerOptions](../v8-web-control/contourlayeroptions-object.md))       |                     | Sets the options of the contour layer.                                      |
| `setVisible(show: boolean)` | | Sets the visibility of the layer. |
| `setZIndex(idx: number)` | | Sets the zIndex of the layer. See also: [zIndexing in Bing Maps V8](../v8-web-control/zindexing-in-bing-maps-v8.md)  |

## Events ##


| Name   | Arguments    | Description   |
|--------|--------------|---------------|
| `click`      | [LayerMouseEventArgs](LayerMouseEventArgs%20Object.md) | Occurs when the mouse is used to click the map or when a touch end event occurs on a contour line in the layer.               |
| `dblclick` | [LayerMouseEventArgs](LayerMouseEventArgs%20Object.md)| Occurs when the mouse is used to double click the map or when a touch end event occurs on a contour line in the layer. |
| `mousedown`  | [LayerMouseEventArgs](LayerMouseEventArgs%20Object.md) | Occurs when the left mouse button is pressed or a touch start event occurs on a contour line in the layer.                    |
| `mouseover`  | [LayerMouseEventArgs](LayerMouseEventArgs%20Object.md) | Occurs when the mouse cursor moves over top of the area covered by a contour line in the layer.                               |
| `mouseout`   | [LayerMouseEventArgs](LayerMouseEventArgs%20Object.md) | Occurs when the mouse cursor moves out of the area covered by a contour line in the layer.                                    |
| `mouseup`    | [LayerMouseEventArgs](LayerMouseEventArgs%20Object.md) | Occurs when the left mouse button is lifted up or when the touch end event occurs on a contour line  in the layer.             |
| `rightclick` | [LayerMouseEventArgs](LayerMouseEventArgs%20Object.md) | Occurs when the right mouse button is used to click the map or when a long touch press occurs on a contour line in the layer. |
