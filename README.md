# FSCSS CamelCase Properties

A comprehensive FSCSS library that enables writing CSS properties in JavaScript-style camelCase notation, automatically converting them to their standard kebab-case equivalents.

## Overview

This library provides a simple and elegant way to write CSS in FSCSS using camelCase property names, making your styles more consistent with JavaScript coding conventions. It includes support for over 500 CSS properties, covering everything from basic layout to modern CSS features.

## Features

- **500+ CSS Properties** - Comprehensive coverage of CSS properties
- **Automatic Conversion** - camelCase to kebab-case conversion
- **Easy Integration** - Simple import and usage
- **Modern CSS Support** - Includes Grid, Flexbox, Container Queries, and more
- **Type-Safe** - Works seamlessly with FSCSS's type system

## Installation

### Basic Import (FSCSS 1.1.16+)

```fscss
// Import the camelCase converter
@import((camelCase) from camelCase))

// Or import everything
@import((*) from camelCase))
```

Legacy Import (fscss standard)

```fscss
@import(exec(_init camelCase))
```

Usage

Basic Example

```fscss
@import((camelCase) from camelCase))

body {
  backgroundColor: #f0f0f0;
  fontFamily: 'Arial', sans-serif;
  fontSize: 16px;
  lineHeight: 1.5;
  margin: 0;
  padding: 20px;
}

.container {
  display: flex;
  flexDirection: column;
  justifyContent: center;
  alignItems: center;
  gap: 16px;
  borderRadius: 8px;
  boxShadow: 0 2px 4px rgba(0,0,0,0.1);
}
```

Advanced Example with Modern CSS

```fscss
@import((camelCase) from camelCase))

.card {
  /* Layout */
  display: grid;
  gridTemplateColumns: repeat(3, 1fr);
  gap: 24px;
  
  /* Spacing */
  padding: 20px;
  marginBottom: 16px;
  
  /* Styling */
  backgroundColor: white;
  borderRadius: 12px;
  boxShadow: 0 4px 6px rgba(0,0,0,0.1);
  
  /* Typography */
  fontFamily: 'Inter', system-ui;
  fontSize: 14px;
  fontWeight: 500;
  lineHeight: 1.4;
  
  /* Animations */
  transition: all 0.3s ease;
  transitionProperty: transform, boxShadow;
  
  &:hover {
    transform: translateY(-4px);
    boxShadow: 0 8px 12px rgba(0,0,0,0.15);
  }
}
```

## Supported Properties

**Layout & Display**

* display
* position
* top, right, bottom, left
* zIndex
* float
* clear
* visibility
* opacity

Flexbox

* flexDirection
* justifyContent
* alignItems
* flexWrap
* flexGrow
* flexShrink
* flexBasis
* order
* gap
* rowGap
* columnGap

**Grid**

* gridTemplateColumns
* gridTemplateRows
* gridAutoColumns
* gridAutoRows
* gridAutoFlow
* gridGap
* gridRow
* gridColumn

**Spacing**

* margin, marginTop, marginRight, marginBottom, marginLeft
* padding, paddingTop, paddingRight, paddingBottom, paddingLeft
* inset, insetBlock, insetInline

**Sizing**

* width, minWidth, maxWidth
* height, minHeight, maxHeight
* aspectRatio

**Typography**

* color
* fontFamily
* fontSize
* fontWeight
* fontStyle
* lineHeight
* textAlign
* textDecoration
* textTransform
* letterSpacing
* wordSpacing
* whiteSpace
* wordBreak
* textOverflow

**Background & Borders**

* backgroundColor
* backgroundImage
* backgroundSize
* backgroundPosition
* backgroundRepeat
* border, borderWidth, borderStyle, borderColor
* borderRadius
* borderTopLeftRadius, borderTopRightRadius, etc.
* boxShadow

**Effects**

· transform
· transformOrigin
· transition
· animation
· filter
· backdropFilter
· mixBlendMode

Modern CSS Features

· container, containerName, containerType
· contentVisibility
· viewTransitionName
· colorScheme
· overscrollBehavior
· scrollBehavior
· scrollSnapType
· touchAction

SVG & Graphics

· fill
· stroke
· strokeWidth
· clipPath
· mask, maskImage

Complete Properties List

<details>
<summary>Click to view all supported properties (500+)</summary>

```javascript
backgroundColor
textAlign
fontSize
fontWeight
lineHeight
marginTop
paddingLeft
borderWidth
borderRadius
boxShadow
textDecoration
whiteSpace
zIndex
flexDirection
justifyContent
alignItems
gridTemplateColumns
columnGap
transitionProperty
animationName
position
top
right
bottom
left
display
visibility
opacity
width
minWidth
maxWidth
height
minHeight
maxHeight
margin
marginRight
marginBottom
marginLeft
padding
paddingTop
paddingRight
paddingBottom
paddingLeft
border
borderTop
borderRight
borderBottom
borderLeft
borderColor
borderStyle
background
backgroundImage
backgroundSize
backgroundRepeat
backgroundPosition
color
fontFamily
fontStyle
fontVariant
letterSpacing
wordSpacing
textTransform
textIndent
overflow
overflowX
overflowY
cursor
pointerEvents
userSelect
flexWrap
flexGrow
flexShrink
flexBasis
alignContent
alignSelf
order
gridGap
gridRow
gridColumn
gridTemplateRows
gridAutoFlow
boxSizing
content
transform
transformOrigin
transition
transitionDuration
transitionTimingFunction
transitionDelay
animationDuration
animationTimingFunction
animationDelay
animationIterationCount
animationDirection
animationFillMode
filter
backdropFilter
mixBlendMode
textShadow
clipPath
maskImage
caretColor
scrollBehavior
scrollSnapType
textFillColor
objectFit
objectPosition
float
clear
listStyle
listStyleType
listStylePosition
listStyleImage
tableLayout
borderCollapse
borderSpacing
emptyCells
captionSide
verticalAlign
direction
unicodeBidi
writingMode
textOrientation
wordBreak
wordWrap
textOverflow
lineBreak
hyphens
quotes
counterReset
counterIncrement
resize
outline
outlineWidth
outlineStyle
outlineColor
outlineOffset
columnCount
columnWidth
columnRule
columnRuleWidth
columnRuleStyle
columnRuleColor
columnSpan
columnFill
perspective
perspectiveOrigin
backfaceVisibility
transformStyle
transformBox
animationPlayState
animationTimeline
scrollMargin
scrollMarginTop
scrollMarginRight
scrollMarginBottom
scrollMarginLeft
scrollPadding
scrollPaddingTop
scrollPaddingRight
scrollPaddingBottom
scrollPaddingLeft
scrollSnapAlign
scrollSnapStop
scrollbarWidth
scrollbarColor
overscrollBehavior
overscrollBehaviorX
overscrollBehaviorY
isolation
breakBefore
breakAfter
breakInside
orphans
widows
fill
stroke
strokeWidth
strokeDasharray
strokeDashoffset
strokeLinecap
strokeLinejoin
strokeMiterlimit
markerStart
markerMid
markerEnd
paintOrder
vectorEffect
shapeOutside
shapeMargin
shapeImageThreshold
clip
all
initial
inherit
unset
revert
lineClamp
olverflowScrolling
tapHighlightColor
textSizeAdjust
touchCallout
userDrag
osxFontSmoothing
overflowStyle
touchAction
borderTopLeftRadius
borderTopRightRadius
borderBottomRightRadius
borderBottomLeftRadius
borderTopColor
borderRightColor
borderBottomColor
borderLeftColor
borderTopWidth
borderRightWidth
borderBottomWidth
borderLeftWidth
borderTopStyle
borderRightStyle
borderBottomStyle
borderLeftStyle
backgroundClip
backgroundOrigin
backgroundAttachment
gap
rowGap
gridAutoColumns
gridAutoRows
justifyItems
justifySelf
inset
insetBlock
insetInline
marginBlock
marginInline
marginBlockStart
marginBlockEnd
marginInlineStart
marginInlineEnd
paddingBlock
paddingInline
paddingBlockStart
paddingBlockEnd
paddingInlineStart
paddingInlineEnd
borderBlock
borderInline
borderBlockStart
borderBlockEnd
borderInlineStart
borderInlineEnd
borderBlockColor
borderBlockStyle
borderBlockWidth
fontKerning
fontFeatureSettings
fontVariationSettings
textCombineUpright
textDecorationColor
textDecorationLine
textDecorationStyle
textDecorationThickness
textUnderlineOffset
textEmphasis
textEmphasisColor
textEmphasisStyle
translate
rotate
scale
transitionBehavior
animationComposition
overflowAnchor
overflowClipMargin
appearance
forcedColorAdjust
colorScheme
contain
containIntrinsicSize
containIntrinsicWidth
containIntrinsicHeight
container
containerName
containerType
viewTransitionName
contentVisibility
mathStyle
mathDepth
aspectRatio
mask
maskType
maskComposite
maskMode
maskPosition
maskRepeat
maskSize
maskClip
maskOrigin
willChange
counterSet
page
pageBreakBefore
pageBreakAfter
pageBreakInside
insetBlockStart
insetBlockEnd
insetInlineStart
insetInlineEnd
colorMix
```

</details>

Version Compatibility

· FSCSS 1.1.20+ - Fully supported (recommended)
· FSCSS 1.1.16+ - Supported
· Earlier versions - Use legacy import syntax

Benefits

1. Consistency: Write CSS properties like JavaScript variables
2. Productivity: Less typing and fewer hyphens
3. IDE Friendly: Better autocomplete support in editors
4. Modern: Includes support for the latest CSS features
5. Complete: Over 500 properties covered

Contributing

Feel free to submit issues or pull requests to add more properties or improve the library.

License

MIT

Support

For issues or questions, please open an issue on the GitHub repository.

---

Made with ❤️ for the FSCSS community
