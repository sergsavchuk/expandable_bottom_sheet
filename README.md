# ExpandableBottomSheet

*This is a BottomSheet with a draggable height like the Google Maps App on Android.*

<img src="https://github.com/torbenkeller/expandable_bottom_sheet/raw/assets/expandable_bottom_sheet_easy.gif"> | <img src="https://github.com/torbenkeller/expandable_bottom_sheet/raw/assets/expandable_bottom_sheet_expert.gif">

## How to use it?
Just look into the [example Tab](https://pub.dev/packages/expandable_bottom_sheet#-example-tab-)

## Arguments

Argument | Description
--- | ---
expandableContent | This is the widget which you can hide and show by dragging. It has to be a widget with a constant height.
background | This is the widget behind the `expandableContent` which holds usually the content of your page.
persistentHeader | This is a Widget which is on top of the `expandableContent` and will never be hidden. It is made for a widget which indicates the user he can expand the content by dragging.
persistentFooter | This is a widget which is always shown at the bottom. The `expandableContent`is if it is expanded on top of it so you don't need margin to see all of your content. You can use it for example for navigation or a menu.
persistentContentHeight | This is the height of the content which will never been contracted. It only relates to `expandableContent`. `persistentHeader` and `persistentFooter` will not be affected by this.
animationDurationExtend | This is the duration for the animation if you stop dragging with high speed.
animationDurationContract | is the duration for the animation to bottom if you stop dragging with high speed. If it is `null` `animationDurationExtend` will be used.
animationCurveExpand | This is the curve of the animation for expanding the `expandableContent` if the drag ended with high speed.
animationCurveContract | This is the curve of the animation for contracting the `expandableContent` if the drag ended with high speed.
onIsExtendedCallback | This will be executed if the extend reaches its maximum.
onIsContractedCallback | This will be executed if the extend reaches its minimum.